---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc07474256eb8a8d5c4ed543648a2eeb55cc7320
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719227"
---
```powershell

Import-Module Microsoft.Graph.Search

$params = @{
    DisplayName = "Global Country Holidays"
    WebUrl = "http://www.contoso.com/"
    Description = "The dates that Contoso offices will be closed to observe holidays. These dates may differ from the actual date of the holiday in cases where the holiday falls on a weekend.    <table>    <thead>    <tr>    <td><strong>2021 Dates</strong></td>    <td><strong>Holiday</strong></td>    </tr>    </thead>    <tbody>    <tr>        <td>January 1, 2021</td>        <td>New Year's Day</td>    </tr>        <tr>        <td>January 18, 2021</td>        <td>Martin Luther King Day</td>    </tr>        <tr>        <td>February 15, 2021</td>        <td>Presidents Day</td>    </tr>        <tr>        <td>May 31, 2021</td>        <td>Memorial Day</td>    </tr>        <tr>        <td>July 5, 2021</td>        <td>Independence Day</td>    </tr>        <tr>        <td>September 6, 2021</td>        <td>Labor Day</td>    </tr>        <tr>        <td>November 25, 2021 - November 26, 2021</td>        <td>Thanksgiving Day and Day after Thanksgiving</td>    </tr>    <tr>        <td>December 23, 2021 - December 24, 2021</td>        <td>Christmas Eve and Christmas Day</td>    </tr>    </tbody>    </table>"
    Keywords = @{
        Keywords = @(
            "new years day"
            "martin luther king day"
            "presidents day"
            "memorial day"
            "independence day"
            "labor day"
            "thanksgiving"
            "christmas"
        )
        ReservedKeywords = @(
            "holidays"
            "paid days off"
        )
        MatchSimilarKeywords = $true
    }
    AvailabilityStartDateTime = [System.DateTime]::Parse("2020-09-21T20:01:37Z")
    AvailabilityEndDateTime = [System.DateTime]::Parse("2021-12-31T20:01:37Z")
    LanguageTags = @(
        "en-us"
    )
    Platforms = @(
        "ios"
    )
    State = "published"
}

New-MgSearchQna -BodyParameter $params

```