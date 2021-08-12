---
title: 使用 Microsoft Graph 中的活动源 API 启用跨设备体验
description: 如果你使用活动，这些 Microsoft 体验可以开始在应用中推动交互。 此外，还可以在应用中显示这些活动，以帮助用户恢复他们之前在任何平台（包括 Windows、Android 和 iOS）、任何设备上所做的操作。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: c447d91aa981b729372cb9e4b790b5b03de756bd08f493e00f7acd1c46ba2eff
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182299"
---
# <a name="using-the-activity-feed-api-in-microsoft-graph-to-enable-cross-device-experiences"></a>使用 Microsoft Graph 中的活动源 API 启用跨设备体验

活动有助于用户跨设备快速继续执行应用中的重要任务，从而提高工作效率。 Microsoft 通过诸如 Windows Timeline、Windows Sets、Cortana“从我离开的位置继续”和 Microsoft Launcher 的体验帮助提高用户应用的生产力，这些应用均由活动源驱动。 如果你使用活动，这些 Microsoft 体验可以开始在应用中推动交互。 此外，还可以在应用中显示这些活动，以帮助用户恢复他们之前在任何平台（包括 Windows、Android 和 iOS）、任何设备上所做的操作。

## <a name="why-integrate-with-activities"></a>为什么与这些活动集成？
### <a name="enable-experiences-that-flow-seamlessly-between-windows-android-linux-and-ios-devices"></a>能够实现在 Windows、Android、Linux 和 iOS 设备之间无缝转换的体验 
优质应用有助于用户执行重要操作，便于实现大量创意、生产力和娱乐方案。 继续执行任务可能充满挑战，尤其是当用户要在其他设备或平台上继续执行任务时。 通过将活动集成到应用中，可以帮助用户使用任意方便的屏幕快速返回到最近的任务，即在 Web、移动和桌面之间来回切换。 借助历史记录项，用户可以轻松查看最近使用的活动、何时使用以及使用时长。   

每个用户活动都表示为应用内的一个目标：产品页、电视节目、文档或在游戏中的当前市场活动。 只需一个深层链接即可继续应用中的活动。 [获取最近活动](/graph/api/projectrome-get-recent-activities?view=graph-rest-1.0)可用于创建购物应用的最近查看产品列表，或创建当前阅读的书籍和新闻文章列表。 

### <a name="create-richer-activities-for-any-experience-with-adaptive-cards"></a>使用自适应卡片创建适用于任何体验的更丰富活动
在 Windows Timeline 等 Microsoft 体验中呈现的活动使用[自适应卡片](https://adaptivecards.io/)框架进行显示，这样就可以创建精美、丰富的卡片来展示应用活动了。 也可以使用自适应卡片 SDK 在自己的应用中呈现丰富卡片。 如果没有为每个活动提供一个自适应卡片，我们将基于你的应用程序名称和图标、必填的“标题”字段和可选“描述”字段来自动创建一个简单的活动卡片。 

### <a name="let-microsoft-help-drive-app-usage-with-features-that-reach-hundreds-of-millions-of-customers"></a>让 Microsoft 通过可服务于数亿客户的功能来帮助提升应用的使用率
与用户活动集成不仅能使用户无缝地继续应用中的活动，而且还意味着可以利用一组不断发展的适用于 Windows、iOS 和 Android 的 Microsoft 体验，这些体验旨在提高用户生产力并帮助用户在所有设备上与应用互动。 通过使用 Microsoft Graph，可仅与用户活动进行一次集成，即可服务于数亿消费者和组织中使用 Windows 以及适用于 iOS 和 Android 设备的 Microsoft 产品的数千万客户。

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 中的跨设备体验](cross-device-concept-overview.md)
- [使用活动源 API 继续用户跨设备的活动](/graph/api/resources/activity-feed-api-overview?view=graph-rest-1.0)
- [通过一个请求使用深层插入发布活动和历史记录项](/graph/api/projectrome-put-activity?view=graph-rest-1.0#example-2---deep-insert)
- [详细了解 Project Rome](/windows/project-rome/)