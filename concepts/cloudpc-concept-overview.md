---
title: Microsoft Windows 上的 365 云电脑Graph
description: Windows 365 是一项基于云的服务，它以虚拟机为最终用户设置和托管云电脑。
author: cohanley
ms.localizationpriority: medium
ms.prod: cloud-pc
ms.openlocfilehash: f0c8f2fe2e197a1f0b44d532e09438c889e5dc24
ms.sourcegitcommit: 2e94beae05043a88b389349f0767e3a657415e4c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/19/2021
ms.locfileid: "61124146"
---
# <a name="overview-for-windows-365-cloud-pc-on-microsoft-graph-preview"></a>Microsoft Windows 预览版上的 Graph (365 云) 

Windows 365 是一项基于云的服务，它以虚拟机为最终用户设置和托管云电脑。 管理员可以轻松设置、管理和扩展 365 Windows 365 云电脑，以满足组织的需求。 各个最终用户可以使用其 Windows 365 云电脑随时将丰富的个性化 Windows 体验（包括他们的应用、数据、内容和设置）从 Microsoft 云安全流式传输到任何设备。

## <a name="why-integrate-with-windows-365-cloud-pcs"></a>为什么与 Windows 365 云电脑集成？ 

通过集成 365 Windows构建，你可以尽快、轻松地为最终用户预配、管理和保护云电脑。 使用 Microsoft Graph API，你可以预配云电脑、管理设备映像、在本地网络连接上创建和运行运行状况检查、创建和分配预配策略等。  

### <a name="create-on-premises-network-connections"></a>创建本地网络连接

创建 [本地网络连接，](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true) 使域控制器看到。 创建后，如果未使用，可以删除本地网络连接。 此外，还可以在本地网络连接上运行运行状况检查，以检查其运行状况，并根据需要更新 AD 域密码。 

### <a name="provision-cloud-pcs"></a>预配云电脑

创建 [预配策略并](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true) 分配给用户组，以在分配许可证时为其预配云电脑。 设置策略创建后，还可以列出、更新和删除设置策略。 

### <a name="upload-device-images"></a>Upload设备映像

Upload和管理云电脑的操作系统映像，以确定[](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true)哪个版本的 Windows预配时，哪些应用和其他图像详细信息应该用于云电脑。  

### <a name="view-end-users-cloud-pcs-and-their-properties"></a>查看最终用户的云电脑及其属性

预配后，列出和查看最终用户的 [云电脑](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) 以及所有关联的属性。 此云电脑可见性支持动手管理并根据需要轻松进行疑难解答。 

## <a name="api-reference"></a>API 参考

正在查找服务的 API 参考？
- [通过 Microsoft Graph API 使用 Windows 365 云电脑](/graph/api/resources/cloudpc-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-step"></a>后续步骤

- 使用 Microsoft Windows资源管理器试用 Graph 365[云电脑 API。](https://developer.microsoft.com/graph/graph-explorer)
