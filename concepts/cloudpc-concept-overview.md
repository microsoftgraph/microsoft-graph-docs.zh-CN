---
title: Microsoft Graph (预览版) 上的Windows 365 云电脑
description: 与Windows 365 云电脑集成，创建 Azure 网络连接、预配云电脑、管理设备映像以及创建和分配预配策略。
author: cohanley
ms.localizationpriority: medium
ms.prod: cloud-pc
ms.openlocfilehash: 75d67a10b12d15430c61a30bedc25eb5a8ab1bb6
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442139"
---
# <a name="overview-for-windows-365-cloud-pc-on-microsoft-graph-preview"></a>Microsoft Graph 上Windows 365 云电脑 (预览版) 概述

Windows 365是基于云的服务，可将云电脑预配并托管为最终用户的虚拟机。 管理员可以轻松地设置、管理和缩放Windows 365云电脑，以满足组织的需求。 单个最终用户可以随时使用其Windows 365 云电脑安全地将丰富的个性化 Windows 体验&mdash;（包括其应用、数据、内容和设置&mdash;）从 Microsoft 云流式传输到任何设备。

## <a name="why-integrate-with-windows-365-cloud-pcs"></a>为什么要与Windows 365云电脑集成？ 

通过与Windows 365集成和构建，可以尽快轻松地为最终用户预配、管理和保护云电脑。 使用 Microsoft 图形 API，可以预配云电脑、管理设备映像、在 Azure 网络连接上创建和运行运行状况检查、创建和分配预配策略等。  

### <a name="create-azure-network-connections"></a>创建 Azure 网络连接

创建 [Azure 网络连接](/graph/api/resources/cloudpconpremisesconnection?view=graph-rest-beta&preserve-view=true) ，为域控制器提供视线。 创建后，如果未使用，则可以删除 Azure 网络连接。 还可以在 Azure 网络连接上运行运行运行状况检查，以检查其运行状况，如果需要，可以更新 Active Directory 域密码。 

### <a name="provision-cloud-pcs"></a>预配云电脑

创建 [预配策略，](/graph/api/resources/cloudpcprovisioningpolicy?view=graph-rest-beta&preserve-view=true) 并分配给用户组，以便在分配了许可证时向其预配云电脑。 创建预配策略后，还可以列出、更新和删除预配策略。 

### <a name="upload-device-images"></a>上传设备映像

上传和管理云电脑的操作系统 [映像](/graph/api/resources/cloudpcdeviceimage?view=graph-rest-beta&preserve-view=true) ，以确定预配时应将哪些应用和其他映像详细信息用于云电脑的 Windows 版本。  

### <a name="view-end-users-cloud-pcs-and-their-properties"></a>查看最终用户的云电脑及其属性

预配后，列出并查看最终用户的 [云电脑](/graph/api/resources/cloudpc?view=graph-rest-beta&preserve-view=true) 和所有关联属性。 此云电脑可见性允许动手管理和在需要时轻松进行故障排除。 

## <a name="api-reference"></a>API 参考

查找服务的 API 参考？

- [通过 Microsoft Graph API 使用 Windows 365 云电脑](/graph/api/resources/cloudpc-api-overview?view=graph-rest-beta&preserve-view=true)

## <a name="next-step"></a>后续步骤

- 使用[图形资源管理器](https://developer.microsoft.com/graph/graph-explorer)试用Windows 365 云电脑 API。
