## API Endpoints Structure ## 

### Authentication
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout
- `GET /api/auth/verify` - Verify JWT token

### Search
- `GET /api/search/stops?query={text}` - Search stops (autocomplete)
- `POST /api/search/trips` - Search trips between stops

### Real-time Data
- `GET /api/realtime/departures/:stopId` - Get departures from stop
- `GET /api/realtime/arrivals/:stopId` - Get arrivals to stop
- `GET /api/realtime/trip/:tripId` - Get real-time trip updates

### Vehicle Tracking
- `GET /api/vehicle/positions/:operator` - Get vehicle positions
- `GET /api/vehicle/track/:vehicleId` - Track specific vehicle (Oxyfi)

### Booking
- `POST /api/booking/create` - Create booking & generate ticket
- `GET /api/booking/:bookingId` - Get booking details
- `GET /api/booking/:bookingId/pdf` - Download ticket PDF
