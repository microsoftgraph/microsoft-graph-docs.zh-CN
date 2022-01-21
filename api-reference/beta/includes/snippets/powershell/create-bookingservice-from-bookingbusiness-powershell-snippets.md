---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 406aa0a7ca81528333cdd6a91bef4fd9f5881095
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113998"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    "@odata.type" = "#microsoft.graph.bookingService"
    DefaultDuration = "PT1H30M"
    DefaultLocation = @{
        "@odata.type" = "#microsoft.graph.location"
        Address = @{
            "@odata.type" = "#microsoft.graph.physicalAddress"
            City = "Buffalo"
            CountryOrRegion = "USA"
            PostalCode = "98052"
            PostOfficeBox = $null
            State = "NY"
            Street = "4567 First Street"
            "Type@odata.type" = "#microsoft.graph.physicalAddressType"
            Type = $null
        }
        Coordinates = $null
        DisplayName = "Contoso Lunch Delivery"
        LocationEmailAddress = $null
        "LocationType@odata.type" = "#microsoft.graph.locationType"
        LocationType = $null
        LocationUri = $null
        UniqueId = $null
        "UniqueIdType@odata.type" = "#microsoft.graph.locationUniqueIdType"
        UniqueIdType = $null
    }
    DefaultPrice = 10
    "DefaultPriceType@odata.type" = "#microsoft.graph.bookingPriceType"
    DefaultPriceType = "fixedPrice"
    "DefaultReminders@odata.type" = "#Collection(microsoft.graph.bookingReminder)"
    DefaultReminders = @(
        @{
            "@odata.type" = "#microsoft.graph.bookingReminder"
            Message = "Please be reminded that this service is tomorrow."
            Offset = "P1D"
            "Recipients@odata.type" = "#microsoft.graph.bookingReminderRecipients"
            Recipients = "allAttendees"
        }
    )
    Description = "Individual bento box lunch delivery"
    DisplayName = "Bento"
    IsLocationOnline = $true
    SmsNotificationsEnabled = $true
    IsHiddenFromCustomers = $false
    Notes = "Home-cooked special"
    PostBuffer = "PT10M"
    PreBuffer = "PT5M"
    SchedulingPolicy = @{
        "@odata.type" = "#microsoft.graph.bookingSchedulingPolicy"
        AllowStaffSelection = $true
        MaximumAdvance = "P10D"
        MinimumLeadTime = "PT10H"
        SendConfirmationsToOwner = $true
        TimeSlotInterval = "PT1H"
    }
    "StaffMemberIds@odata.type" = "#Collection(String)"
    StaffMemberIds = @(
        "d90d1e8c-5cfe-48cf-a2d5-966267375b6a"
        "2f5f8794-0b29-45b5-b56a-2eb5ff7aa880"
    )
}

New-MgBookingBusinessService -BookingBusinessId $bookingBusinessId -BodyParameter $params

```