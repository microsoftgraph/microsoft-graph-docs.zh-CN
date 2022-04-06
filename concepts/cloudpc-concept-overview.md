---
title: Microsoft Windows 365 云电脑 上的 Graph
description: Windows 365是一种基于云的服务，用于为最终用户将云电脑作为虚拟机进行设置和托管。
author: cohanley
ms.localizationpriority: medium
ms.prod: cloud-pc
ms.openlocfilehash: 3aada87e5f1087beb0f62b6fd2972edbcb0e6454
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589329"
---
# <a name="overview-for-windows-365-cloud-pc-on-microsoft-graph-preview"></a>Microsoft Windows 365 云电脑 预览版Graph (概述) 

Windows 365是一种基于云的服务，用于为最终用户将云电脑作为虚拟机进行设置和托管。 管理员可以轻松地设置、管理和扩展Windows 365云电脑以满足组织的需求。 各个最终用户可以使用自己的 Windows，将丰富的个性化体验（包括他们的应用、数据、内容和设置）从 Microsoft 云安全流式传输至任何设备Windows 365 云电脑。

## <a name="why-integrate-with-windows-365-cloud-pcs"></a>为什么与云Windows 365集成？ 

通过集成和构建Windows 365，您可以尽快、轻松地为最终用户预配、管理和保护云电脑。 使用 Microsoft 图形 API，你可以预配云电脑、管理设备映像、在 Azure 网络连接上创建和运行运行状况检查、创建和分配预配策略等。  

### <a name="create-azure-network-connections"></a>创建 Azure 网络连接

创建 [Azure 网络连接](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true) ，使域控制器看到。 创建后，如果未使用，可以删除 Azure 网络连接。 还可以在 Azure 网络连接上运行运行状况检查，以检查其运行状况，并根据需要更新 AD 域密码。 

### <a name="provision-cloud-pcs"></a>预配云电脑

创建 [预配策略并](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true) 分配给用户组，以在分配许可证时为其预配云电脑。 设置策略创建后，还可以列出、更新和删除设置策略。 

### <a name="upload-device-images"></a>Upload设备映像

Upload和管理云电脑的操作系统映像，[](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true)以确定在预配时Windows哪些应用和其他图像详细信息应用于云电脑。  

### <a name="view-end-users-cloud-pcs-and-their-properties"></a>查看最终用户的云电脑及其属性

预配后，列出和查看最终用户的 [云电脑](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) 以及所有关联的属性。 此云电脑可见性支持动手管理并根据需要轻松进行疑难解答。 

## <a name="api-reference"></a>API 参考

正在查找服务的 API 参考？
- [通过 Microsoft Graph API 使用 Windows 365 云电脑](/graph/api/resources/cloudpc-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-step"></a>后续步骤

- 使用 Microsoft Windows 365资源管理器试用[云Graph API](https://developer.microsoft.com/graph/graph-explorer)。
