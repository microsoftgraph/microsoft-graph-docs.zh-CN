---
title: OneDrive 活动报表
description: 您可以获取许可使用 OneDrive 看它们与 OneDrive 上的文件的交互的每个用户的活动。 此外可帮助您了解协作事通过显示共享的文件数的级别。
ms.openlocfilehash: cfcae36cad301c777eea4ede4532efda0ce13b39
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049130"
---
# <a name="onedrive-activity-reports"></a>OneDrive 活动报表

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

您可以获取许可使用 OneDrive 看它们与 OneDrive 上的文件的交互的每个用户的活动。 此外可帮助您了解协作事通过显示共享的文件数的级别。

> **注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。

## <a name="reports"></a>报表

| 函数                                 | CSV 返回类型 | JSON 返回类型                         | 说明                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [获取用户详细信息](../api/reportroot-getonedriveactivityuserdetail.md) | Stream          | [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) | 获取用户执行的 OneDrive 活动的详细信息。 |
| [获取用户数](../api/reportroot-getonedriveactivityusercounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | 获取 OneDrive 活跃用户数趋势。 |
| [获取文件数](../api/reportroot-getonedriveactivityfilecounts.md) | Stream          | [siteActivitySummary](../resources/siteactivitysummary.md) | 获取对任意 OneDrive 帐户执行文件交互的唯一许可用户数。 |
