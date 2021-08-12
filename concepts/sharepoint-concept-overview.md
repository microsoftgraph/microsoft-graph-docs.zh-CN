---
title: SharePoint 网站和内容 API 概述
description: SharePoint 是移动且智能的内部网。 借助 SharePoint，用户可以共享和管理内容、知识和应用程序，以增强团队合作、查找信息并在整个组织内进行协作。 你可以在 Microsoft Graph 中使用 SharePoint REST API，将解决方案与 SharePoint 网站和内容进行集成。
localization_priority: Priority
ms.prod: sharepoint
ms.custom: scenarios:getting-started
ms.openlocfilehash: 1771ff2513e255fbec6a252881cf25a92fead91fe21a42820334424520a697f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54235070"
---
# <a name="sharepoint-sites-and-content-api-overview"></a>SharePoint 网站和内容 API 概述

SharePoint 是移动且智能的内部网。 借助 SharePoint，用户可以共享和管理内容、知识和应用程序，以增强团队合作、查找信息并在整个组织内进行协作。 你可以在 Microsoft Graph 中使用 SharePoint REST API，将解决方案与 SharePoint 网站和内容进行集成。

## <a name="why-integrate-with-sharepoint-sites-and-content"></a>为什么与 SharePoint 网站和内容集成？

SharePoint 网站可增强团队的协作和沟通。 Microsoft 365 组、Microsoft Teams 和门户均基于 SharePoint，因此，可以使用 Microsoft Graph 来访问数据，而无需考虑数据存储在何处。 在 Microsoft Graph 中使用 SharePoint API 可访问：

- 存储用户与其同事协作内容的团队网站。
- 用户发布要在整个组织中共享的丰富内容页的通信网站和门户。

### <a name="unleash-your-data-with-sharepoint-lists"></a>借助 SharePoint 列表充分使用数据

[列表][list]是 SharePoint 中数据存储的基础。
[创建列表][create]以存储各种不同的业务数据，从简单的客户联系人列表到前端具有 PowerApps 的自定义业务应用程序。
使用[列][]定义架构时，SharePoint 可以保护数据的完整性，并启用丰富的索引、查询和搜索功能。

### <a name="bring-the-power-of-lists-to-your-teams-files"></a>将列表的强大功能引入团队文件中

SharePoint 将文件存储在名为文档库的特殊[列表类型][]中。
可以使用 [OneDrive API][] 将库用作[驱动器][]，或使用 SharePoint API 将库用作[列表][]。
就像常规列表一样，可以扩展文档库的架构以通过自定义列来支持业务需求。

### <a name="light-up-your-app-with-your-users-sharepoint-intranet-data"></a>通过用户的 SharePoint 内部网数据使应用更强大

使用 Microsoft Graph，可以在应用中显示用户最重要的数据。
通过[查询][]存储用户数据的列表来使数据保持最新。
为应用[创建][]自己的列表，并允许用户在其他 SharePoint 体验中访问你的数据，或使数据处于隐藏状态。

### <a name="use-microsoft-graph-to-extend-sharepoint"></a>使用 Microsoft Graph 扩展 SharePoint

作为平台，SharePoint 提供一些用于扩展和集成的模型：

- [SharePoint Framework][] 提供了一种方法，使用可托管于 SharePoint 页面上的客户端技术和开源代码工具生成 Web 部件。
- [SharePoint 外接程序][]是可添加到 SharePoint 网站而无需在服务器上运行自定义代码的自包含扩展。

当应用在 SharePoint 页面内运行时，可以使用 Microsoft Graph 轻松访问整个 Microsoft 365 中的数据。

若要详细了解这些模型，请访问 [SharePoint 开发人员中心][]或 [SharePoint 开发人员文档][]。

## <a name="api-reference"></a>API 参考
在查找此服务的 API 参考？

- [Microsoft Graph v1.0 中的 SharePoint API](/graph/api/resources/sharepoint?view=graph-rest-1.0)
- [Microsoft Graph beta 中的 SharePoint API](/graph/api/resources/sharepoint?view=graph-rest-beta)

## <a name="next-steps"></a>后续步骤

详细了解[使用网站](/graph/api/resources/sharepoint?view=graph-rest-1.0)，开始在 Microsoft Graph 中使用 SharePoint。

[list]: /graph/api/resources/list?view=graph-rest-1.0
[列]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[列表类型]: /graph/api/resources/listinfo?view=graph-rest-1.0
[创建]: /graph/api/list-create?view=graph-rest-1.0
[查询]: /graph/api/listitem-get?view=graph-rest-1.0
[驱动器]: /graph/api/resources/drive?view=graph-rest-1.0
[OneDrive API]: /graph/api/resources/onedrive?view=graph-rest-1.0
[SharePoint Framework]: /sharepoint/dev/spfx/sharepoint-framework-overview
[SharePoint 外接程序]: /sharepoint/dev/sp-add-ins/sharepoint-add-ins
[SharePoint 开发人员中心]: https://developer.microsoft.com/sharepoint
[SharePoint 开发人员文档]: /sharepoint/dev/
[SharePoint]: /graph/api/resources/sharepoint?view=graph-rest-1.0