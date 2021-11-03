---
title: 使用 microsoft Windows API 使用 Graph 365 云电脑
description: 借助 Microsoft Graph，可以在组织中预配和管理云电脑，如果与 Intune API 结合使用，还可以在物理终结点旁边管理云电脑。
author: cohanley
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e4e205631424ed2f93b748371c8f32c31b4398ee
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695424"
---
# <a name="working-with-windows-365-cloud-pcs-using-the-microsoft-graph-api"></a>使用 microsoft Windows API 使用 Graph 365 云电脑

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows 365 是一项基于云的服务，它以虚拟机为最终用户设置和托管云电脑。 管理员可以轻松设置、管理和扩展 365 Windows 365 云电脑，以满足组织的需求。 各个最终用户可以使用其 Windows 365 云电脑随时将丰富的个性化 Windows 体验（包括他们的应用、数据、内容和设置）从 Microsoft 云安全流式传输到任何设备。

Microsoft Graph API 支持以编程方式访问组织的云电脑信息和管理操作。 API 执行的操作与通过 Microsoft Endpoint Manager。 

> [!IMPORTANT]
> 使用适用于Graph的 Microsoft Graph API 需要组织有效的[Windows 365](https://www.microsoft.com/windows-365)许可证。 目前，Microsoft Graph API 适用于 Windows 365 Enterprise，Windows 365 商业版。 

## <a name="using-the-microsoft-graph-api-for-cloud-pcs"></a>使用 Microsoft Graph API 云电脑

借助 Microsoft Graph，可以在组织中预配和管理云电脑。 如果与 Intune API 结合使用，还可以在物理终结点旁边管理云电脑。 

## <a name="using-microsoft-graph-permissions"></a>使用 Microsoft Graph 权限

Microsoft Graph 通过权限控制对资源的访问。 作为开发人员，您必须指定访问 365 资源所需的Windows权限。 通常是在 Azure Active Directory 门户中指定权限。 有关详细信息，请参阅[Microsoft Graph权限参考](/graph/permissions-reference)并导航到[云电脑权限](/graph/permissions-reference#cloud-pc-permissions)部分。 

## <a name="common-use-cases"></a>常见用例

|用例|REST 资源|另请参阅|
|:---|:---|:---|
|列出、获取、创建、更新、删除或分配预配策略|[cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)|[预配概述](/windows-365/enterprise/provisioning)|
|管理云电脑，包括重新预配、结束云电脑宽限期、批量重新预配和调整云电脑大小|[cloudPC](../resources/cloudpc.md)|[云电脑生命周期](/windows-365/enterprise/lifecycle)|
|列出、获取、创建、删除、获取源映像，然后重新加载云电脑操作系统映像|[cloudPCDeviceImage](../resources/cloudpcdeviceimage.md)|[设备映像概述](/windows-365/enterprise/device-images)|
|列出、获取、创建、更新删除、更新 AD 域密码，并运行本地网络连接的运行状况检查|[cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)|[本地网络连接概述](/windows-365/enterprise/on-premises-network-connections)|
|列出云电脑的审核事件、获取特定审核事件和获取审核活动类型|[cloudPcAuditEvent](../resources/cloudpcauditevent.md)|[获取云电脑审核日志](/windows-365/enterprise/get-cloud-pc-audit-logs-using-powershell)|
|列出、获取、创建、更新、删除或分配用户设置|[cloudPcUserSetting](../resources/cloudpcusersetting.md)|[用户设置概述](../resources/cloudpcusersetting.md)|

## <a name="whats-new"></a>最近更新

了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。