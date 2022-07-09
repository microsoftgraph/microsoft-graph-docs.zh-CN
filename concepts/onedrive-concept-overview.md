---
title: OneDrive 文件存储 API 概述
description: '使用 Microsoft 365 中的文件中心 OneDrive 访问文件，无论文件存储在何处。 使用 Microsoft Graph 以使用单个 API 来处理这些文件。 '
ms.localizationpriority: high
ms.prod: onedrive
ms.custom: scenarios:getting-started
ms.openlocfilehash: 311dc13807b63522d6800ae619d310f7395db5e6
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698205"
---
# <a name="onedrive-file-storage-api-overview"></a>OneDrive 文件存储 API 概述

OneDrive 是 Microsoft 365 的文件中心。 人们会在各种各样的环境中使用文件，如 Microsoft Teams、组、SharePoint 等。 通过 OneDrive，用户可以访问这些文件而不管它们存储在什么位置，而通过 Microsoft Graph，则可以使用单个 API 来使用它们。

Microsoft 365 中的文件存储在[驱动器][Drive API]中。 用户可以在个人驱动器（&mdash;其 OneDrive&mdash;）或 [SharePoint][] 文档库支持的共享驱动器中存储文件。 但是 OneDrive 的灵活性可使用户以最佳的方式进行协作。
用户可以共享文件链接、将文件复制或移动到团队驱动器，甚至可以将 OneDrive 文件附加到 Outlook 中的邮件消息。

> [!VIDEO https://www.youtube-nocookie.com/embed/vG-hQxFHCAE]

## <a name="why-integrate-with-onedrive-file-storage-in-the-cloud"></a>为什么与云中的 OneDrive 文件存储集成？

### <a name="tap-into-an-ecosystem-with-billions-of-files"></a>利用一个包含数十亿个文件的生态系统

OneDrive 用户可从任何设备以联机或脱机方式访问他们的文件，并与其组织内外人员共享文件。
OneDrive 可以在 Word、Excel 和 PowerPoint 等熟悉的应用中实现实时共同创作功能。
通过 Microsoft Graph 提供支持的数百种格式、视频流、分析等丰富的缩略图呈现文件。
OneDrive 中的数据受到客户信任的高级加密、合规性和安全性功能的保护。

有超过 5 亿的设备运行 OneDrive 应用，超过 85% 的财富 500 强企业使用 OneDrive for Business，通过将应用与 OneDrive 集成，你可以与数以百万计的消费者、学生和商业用户建立联系，并与每天都在其中工作的客户进行互动。

### <a name="store-your-apps-files-in-a-powerful-cloud"></a>将应用文件存储在功能强大的云中

当你将文件存储在 OneDrive 中时，应用可以利用 Microsoft 云的功能，且你的用户可以在任何地方访问他们的文件。
通过[文件选择器][] SDK，可以使用 OneDrive 用户熟悉的相同体验，快速打开、下载、保存或共享存储在 OneDrive 中的文件。
从选取器 SDK 中直接获取关于选定文件的信息，或者直接使用 Microsoft Graph API 与文件进行更深入的交互。
使用[][]“特殊文件夹”将文件存储在 OneDrive 上的已知位置，如 `Documents` 和 `Camera Roll`，或者为你的应用提供其自己的个人文件夹。

### <a name="bring-your-app-straight-to-users-within-onedrive"></a>在 OneDrive 中直接向用户提供你的应用

OneDrive 客户可以直接在 OneDrive 中使用或启动你的应用，以打开、编辑或预览文件。
使用 OneDrive 的[文件处理程序][]扩展，为你自己的自定义文件扩展名提供图标和预览，将你的应用添加到“新建”按钮，甚至可以将你自己的自定义操作添加到菜单栏以启动应用。

### <a name="work-with-content-in-formats-your-app-understands"></a>使用应用理解的格式来处理内容

应用可以以最方便的格式获取文件内容。
应用可以显示数百种不同文件格式的自定义大小的“缩略图”[][]。
你可以下载各种不同“格式”[][]的文件，如 PDF。
甚至可以在应用中使用[][]预览 API (beta) 嵌入的 OneDrive 文件预览程序。

### <a name="work-with-file-content-and-metadata-without-downloading-the-binary"></a>在不下载二进制文件的情况下使用文件内容和元数据

使用 Microsoft Graph，可以通过 REST API 访问丰富的内容，而无需下载二进制文件。
在[][]“照片”、[][]“音频”和[][]“视频”文件中探索提取的元数据。
使用 Excel API[][] 可直接使用存储在 Excel 工作簿中的原始数据。
使用[][]注释 API 可访问 OneNote 笔记本内容。

### <a name="react-to-file-changes"></a>对文件更改做出反应

通过 webhooks[][]，当文件发生更改时你将收到通知，以此可以快速做出响应。
[delta API][] 可用于查看自上次应用与云同步以来发生的更改。

## <a name="api-reference"></a>API 参考
在查找此服务的 API 参考？

- [Microsoft Graph v1.0 中的 OneDrive 文件存储 API](/graph/api/resources/onedrive)
- [Microsoft Graph beta 中的 OneDrive 文件存储 API](/graph/api/resources/onedrive)

## <a name="next-steps"></a>后续步骤

详细了解如何在 Microsoft Graph v1.0 中[使用 OneDrive API][Drive API]。

[SharePoint]: sharepoint-concept-overview.md
[文件选取器]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[文件处理程序]: /onedrive/developer/file-handlers
[特殊文件夹]: /graph/api/drive-get-specialfolder
[注释 API]: integrate-with-onenote.md
[Excel API]: /graph/api/resources/excel
[REST API]: /graph/api/resources/onedrive
[增量 API]: /graph/api/driveitem-delta
[视频]: /graph/api/resources/video
[照片]: /graph/api/resources/photo
[音频]: /graph/api/resources/audio
[格式]: /graph/api/driveitem-get-content-format
[缩略图]: /graph/api/driveitem-list-thumbnails
[预览]: /graph/api/driveitem-preview
[webhooks]: /graph/api/resources/webhooks
[Drive API]: /graph/api/resources/onedrive