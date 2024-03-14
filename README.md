# plan
class TripPlanner:
    def __init__(self):
        self.destination = ""
        self.departure_date = ""
        self.return_date = ""
        self.transportation = ""
        self.accommodation = ""
        self.activities = []

    def set_destination(self, destination):
        self.destination = destination

    def set_departure_date(self, departure_date):
        self.departure_date = departure_date

    def set_return_date(self, return_date):
        self.return_date = return_date

    def set_transportation(self, transportation):
        self.transportation = transportation

    def set_accommodation(self, accommodation):
        self.accommodation = accommodation

    def add_activity(self, activity):
        self.activities.append(activity)

    def print_trip_details(self):
        print("Trip Details:")
        print("Destination:", self.destination)
        print("Departure Date:", self.departure_date)
        print("Return Date:", self.return_date)
        print("Transportation:", self.transportation)
        print("Accommodation:", self.accommodation)
        print("Activities:")
        for activity in self.activities:
            print("-", activity)


# Example Usage
if __name__ == "__main__":
    trip = TripPlanner()

    trip.set_destination("Paris, France")
    trip.set_departure_date("2024-07-01")
    trip.set_return_date("2024-07-10")
    trip.set_transportation("Flight")
    trip.set_accommodation("Hotel")

    trip.add_activity("Visit Eiffel Tower")
    trip.add_activity("Louvre Museum tour")
    trip.add_activity("Seine River Cruise")

    trip.print_trip_details()
