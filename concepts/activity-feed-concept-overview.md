---
title: 使用活动源 API 启用跨设备体验
description: 使用 Microsoft Graph，可以启用在设备之间无缝流动的体验，使用自适应卡创建更丰富的活动，并帮助推动应用使用。
ms.localizationpriority: medium
ms.prod: project-rome
ms.openlocfilehash: dfe47f0d41ca978bac04a3ce1bb2a5c8889491b4
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437035"
---
# <a name="use-the-activity-feed-api-in-microsoft-graph-to-enable-cross-device-experiences"></a>使用 Microsoft Graph 中的活动源 API 启用跨设备体验

活动有助于用户跨设备快速继续执行应用中的重要任务，从而提高工作效率。 Microsoft 通过 Windows 时间线、Windows 集、Cortana Pick up Where I left off 和 Microsoft Launcher 等体验帮助提高应用的用户工作效率，这些体验都由活动源提供支持。 如果你使用活动，这些 Microsoft 体验可以开始在应用中推动交互。 此外，还可以在应用中显示这些活动，以帮助用户恢复他们之前在任何平台（包括 Windows、Android 和 iOS）、任何设备上所做的操作。

以下部分介绍了与活动集成的好处。

## <a name="enable-experiences-that-flow-seamlessly-between-windows-android-linux-and-ios-devices"></a>能够实现在 Windows、Android、Linux 和 iOS 设备之间无缝转换的体验

出色的应用程序可帮助用户完成各种&mdash;创意、工作效率和娱乐场景。 继续执行任务可能充满挑战，尤其是当用户要在其他设备或平台上继续执行任务时。 通过将活动合并到应用程序中，你可以帮助用户快速返回到最近的任务，使用任何方便的屏幕&mdash;，他们可以从 Web 移动到移动到桌面，然后再次返回。 借助历史记录项，用户可以轻松查看最近使用的活动、何时使用以及使用时长。

每个用户活动都表示为应用内的一个目标：产品页、电视节目、文档或在游戏中的当前市场活动。 只需一个深层链接即可继续应用中的活动。 使用 [“获取最近的活动](/graph/api/projectrome-get-recent-activities) ”创建购物应用最近查看的产品列表或书籍和新闻文章的当前阅读列表。

## <a name="create-richer-activities-for-any-experience-with-adaptive-cards"></a>使用自适应卡片创建适用于任何体验的更丰富活动

在 Windows Timeline 等 Microsoft 体验中呈现的活动使用[自适应卡片](https://adaptivecards.io/)框架进行显示，这样就可以创建精美、丰富的卡片来展示应用活动了。 也可以使用自适应卡片 SDK 在自己的应用中呈现丰富的卡片。 如果没有为每个活动提供一个自适应卡片，我们将基于你的应用程序名称和图标、必填的“标题”字段和可选“描述”字段来自动创建一个简单的活动卡片。

## <a name="let-microsoft-help-drive-app-usage-with-features-that-reach-hundreds-of-millions-of-customers"></a>让 Microsoft 通过可服务于数亿客户的功能来帮助提升应用的使用率

与用户活动集成不仅使用户能够无缝地恢复应用中的活动，还意味着利用一组不断增长的 Windows、iOS 和 Android&mdash;体验，这些体验旨在提高用户的工作效率，并帮助用户在所有设备上使用你的应用。 通过使用 Microsoft Graph，可仅与用户活动进行一次集成，即可服务于数亿消费者和组织中使用 Windows 以及适用于 iOS 和 Android 设备的 Microsoft 产品的数千万客户。

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 中的跨设备体验](cross-device-concept-overview.md)
- [使用活动源 API 继续用户跨设备的活动](/graph/api/resources/activity-feed-api-overview)
- [通过一个请求使用深层插入发布活动和历史记录项](/graph/api/projectrome-put-activity#example-2---deep-insert)
- [详细了解 Project Rome](/windows/project-rome/)
