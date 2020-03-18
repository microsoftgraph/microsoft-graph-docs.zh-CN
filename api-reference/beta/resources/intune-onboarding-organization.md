---
title: 组织资源类型
description: 组织资源表示在租户级别操作和配置的全局设置和资源的实例。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd8481ddea83194c7e1b769c70518c9ddff3f894
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42778013"
---
# <a name="organization-resource-type"></a><span data-ttu-id="7e688-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="7e688-103">organization resource type</span></span>

> <span data-ttu-id="7e688-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7e688-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e688-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7e688-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e688-106">组织资源表示在租户级别操作和配置的全局设置和资源的实例。</span><span class="sxs-lookup"><span data-stu-id="7e688-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="7e688-107">方法</span><span class="sxs-lookup"><span data-stu-id="7e688-107">Methods</span></span>
|<span data-ttu-id="7e688-108">方法</span><span class="sxs-lookup"><span data-stu-id="7e688-108">Method</span></span>|<span data-ttu-id="7e688-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7e688-109">Return Type</span></span>|<span data-ttu-id="7e688-110">说明</span><span class="sxs-lookup"><span data-stu-id="7e688-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e688-111">列出 organizations</span><span class="sxs-lookup"><span data-stu-id="7e688-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="7e688-112">[organization](../resources/intune-onboarding-organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7e688-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="7e688-113">列出 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e688-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="7e688-114">获取组织</span><span class="sxs-lookup"><span data-stu-id="7e688-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="7e688-115">组织</span><span class="sxs-lookup"><span data-stu-id="7e688-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="7e688-116">读取 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7e688-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="7e688-117">更新 organization</span><span class="sxs-lookup"><span data-stu-id="7e688-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="7e688-118">organization</span><span class="sxs-lookup"><span data-stu-id="7e688-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="7e688-119">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7e688-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="7e688-120">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="7e688-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="7e688-121">Int32</span><span class="sxs-lookup"><span data-stu-id="7e688-121">Int32</span></span>|<span data-ttu-id="7e688-122">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="7e688-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="7e688-123">属性</span><span class="sxs-lookup"><span data-stu-id="7e688-123">Properties</span></span>
|<span data-ttu-id="7e688-124">属性</span><span class="sxs-lookup"><span data-stu-id="7e688-124">Property</span></span>|<span data-ttu-id="7e688-125">类型</span><span class="sxs-lookup"><span data-stu-id="7e688-125">Type</span></span>|<span data-ttu-id="7e688-126">说明</span><span class="sxs-lookup"><span data-stu-id="7e688-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e688-127">id</span><span class="sxs-lookup"><span data-stu-id="7e688-127">id</span></span>|<span data-ttu-id="7e688-128">String</span><span class="sxs-lookup"><span data-stu-id="7e688-128">String</span></span>|<span data-ttu-id="7e688-129">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="7e688-129">The GUID for the object.</span></span>|
|<span data-ttu-id="7e688-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="7e688-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="7e688-131">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="7e688-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="7e688-132">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="7e688-132">Mobile device management authority.</span></span> <span data-ttu-id="7e688-133">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="7e688-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="7e688-134">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="7e688-134">certificateConnectorSetting</span></span>|[<span data-ttu-id="7e688-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="7e688-135">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="7e688-136">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="7e688-136">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e688-137">关系</span><span class="sxs-lookup"><span data-stu-id="7e688-137">Relationships</span></span>
<span data-ttu-id="7e688-138">无</span><span class="sxs-lookup"><span data-stu-id="7e688-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e688-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e688-139">JSON Representation</span></span>
<span data-ttu-id="7e688-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e688-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String",
  "certificateConnectorSetting": {
    "@odata.type": "microsoft.graph.certificateConnectorSetting",
    "status": 1024,
    "certExpiryTime": "String (timestamp)",
    "enrollmentError": "String",
    "lastConnectorConnectionTime": "String (timestamp)",
    "connectorVersion": "String",
    "lastUploadVersion": 1024
  }
}
```



