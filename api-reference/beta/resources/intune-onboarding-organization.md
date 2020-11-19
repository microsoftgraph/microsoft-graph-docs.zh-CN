---
title: 组织资源类型
description: 组织资源表示在租户级别操作和配置的全局设置和资源的实例。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30dbbb5b7a86b39acceabc2ebf8df74caafca9c9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259541"
---
# <a name="organization-resource-type"></a><span data-ttu-id="360db-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="360db-103">organization resource type</span></span>

<span data-ttu-id="360db-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="360db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="360db-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="360db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="360db-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="360db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="360db-107">组织资源表示在租户级别操作和配置的全局设置和资源的实例。</span><span class="sxs-lookup"><span data-stu-id="360db-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="360db-108">方法</span><span class="sxs-lookup"><span data-stu-id="360db-108">Methods</span></span>
|<span data-ttu-id="360db-109">方法</span><span class="sxs-lookup"><span data-stu-id="360db-109">Method</span></span>|<span data-ttu-id="360db-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="360db-110">Return Type</span></span>|<span data-ttu-id="360db-111">说明</span><span class="sxs-lookup"><span data-stu-id="360db-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="360db-112">列出 organizations</span><span class="sxs-lookup"><span data-stu-id="360db-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="360db-113">[organization](../resources/intune-onboarding-organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="360db-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="360db-114">列出 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="360db-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="360db-115">获取组织</span><span class="sxs-lookup"><span data-stu-id="360db-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="360db-116">组织</span><span class="sxs-lookup"><span data-stu-id="360db-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="360db-117">读取 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="360db-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="360db-118">更新 organization</span><span class="sxs-lookup"><span data-stu-id="360db-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="360db-119">organization</span><span class="sxs-lookup"><span data-stu-id="360db-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="360db-120">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="360db-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="360db-121">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="360db-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="360db-122">Int32</span><span class="sxs-lookup"><span data-stu-id="360db-122">Int32</span></span>|<span data-ttu-id="360db-123">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="360db-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="360db-124">属性</span><span class="sxs-lookup"><span data-stu-id="360db-124">Properties</span></span>
|<span data-ttu-id="360db-125">属性</span><span class="sxs-lookup"><span data-stu-id="360db-125">Property</span></span>|<span data-ttu-id="360db-126">类型</span><span class="sxs-lookup"><span data-stu-id="360db-126">Type</span></span>|<span data-ttu-id="360db-127">说明</span><span class="sxs-lookup"><span data-stu-id="360db-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="360db-128">id</span><span class="sxs-lookup"><span data-stu-id="360db-128">id</span></span>|<span data-ttu-id="360db-129">String</span><span class="sxs-lookup"><span data-stu-id="360db-129">String</span></span>|<span data-ttu-id="360db-130">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="360db-130">The GUID for the object.</span></span>|
|<span data-ttu-id="360db-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="360db-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="360db-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="360db-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="360db-133">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="360db-133">Mobile device management authority.</span></span> <span data-ttu-id="360db-134">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="360db-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="360db-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="360db-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="360db-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="360db-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="360db-137">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="360db-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="360db-138">关系</span><span class="sxs-lookup"><span data-stu-id="360db-138">Relationships</span></span>
<span data-ttu-id="360db-139">无</span><span class="sxs-lookup"><span data-stu-id="360db-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="360db-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="360db-140">JSON Representation</span></span>
<span data-ttu-id="360db-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="360db-141">Here is a JSON representation of the resource.</span></span>
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




