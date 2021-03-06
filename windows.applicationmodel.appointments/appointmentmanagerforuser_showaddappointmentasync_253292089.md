---
-api-id: M:Windows.ApplicationModel.Appointments.AppointmentManagerForUser.ShowAddAppointmentAsync(Windows.ApplicationModel.Appointments.Appointment,Windows.Foundation.Rect,Windows.UI.Popups.Placement)
-api-type: winrt method
---

<!-- Method syntax
public Windows.Foundation.IAsyncOperation<string> ShowAddAppointmentAsync(Windows.ApplicationModel.Appointments.Appointment appointment, Windows.Foundation.Rect selection, Windows.UI.Popups.Placement preferredPlacement)
-->

# Windows.ApplicationModel.Appointments.AppointmentManagerForUser.ShowAddAppointmentAsync

## -description
Shows the Appointments provider Add Appointment UI, to enable the user to add an appointment.

## -parameters
### -param appointment
The object representing the information for the appointment to add.

### -param selection
The [Rect](../windows.foundation/rect.md) is the rectangular area of user selection (for example, pressing a button), around which the operating system displays the Add Appointment UI, not within that rectangular area. For example, if an app uses a button to show the [Rect](../windows.foundation/rect.md), pass the [Rect](../windows.foundation/rect.md) of the button so the Add Appointment UI displays around the button, not overlapping it.

### -param preferredPlacement
The [Placement](../windows.ui.popups/placement.md) that describes the preferred placement of the Add Appointment UI.

## -returns
When this method completes, it returns a **String** object that represents the appointment. This serves as an appointment identifier for future reference when updating or removing. If the appointment identifier returned is an empty string, the appointment was not added to the Appointments provider app.

## -remarks
When you call this method, the Appointment provider app displays in a light-dismiss pane that is hosted by your app.

> On Windows Phone, this method behaves the same as [ShowEditNewAppointmentAsync](appointmentmanagerforuser_showeditnewappointmentasync_372535555.md), in that the fields in the Add Appointment UI are editable by the user.

## -examples

## -see-also
[ShowAddAppointmentAsync(Appointment, Rect)](appointmentmanagerforuser_showaddappointmentasync_92599717.md)
## -capabilities
appointmentsSystem
