# GooglePlaces-AutoComplete-RecyclerView-Adaper
Don't forget to add in your Activity.


    public static final LatLngBounds BOUNDS_GREATER_SYDNEY = new LatLngBounds(
            new LatLng(-34.041458, 150.790100), new LatLng(-33.682247, 151.383362));

        // Construct a GeoDataClient for the Google Places API for Android.
        mGeoDataClient = Places.getGeoDataClient(getActivity(), null);
     mAdapter = new PlaceAutocompleteRecyclerViewAdapter(getActivity(), mGeoDataClient, Constants.BOUNDS_GREATER_SYDNEY, null);
     
put the below code in Editext Text changed event.
           mAdapter.getFilter().filter(charSequence.toString());
