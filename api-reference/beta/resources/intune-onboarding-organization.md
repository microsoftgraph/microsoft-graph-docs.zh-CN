---
title: 组织资源类型
description: 组织资源表示在租户级别操作和配置的全局设置和资源的实例。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b47ec69063998a935640f05d04a17bfc5714c8d8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398231"
---
# <a name="organization-resource-type"></a><span data-ttu-id="8e633-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="8e633-103">organization resource type</span></span>

> <span data-ttu-id="8e633-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8e633-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8e633-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8e633-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e633-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e633-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e633-107">组织资源表示在租户级别操作和配置的全局设置和资源的实例。</span><span class="sxs-lookup"><span data-stu-id="8e633-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="8e633-108">方法</span><span class="sxs-lookup"><span data-stu-id="8e633-108">Methods</span></span>
|<span data-ttu-id="8e633-109">方法</span><span class="sxs-lookup"><span data-stu-id="8e633-109">Method</span></span>|<span data-ttu-id="8e633-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8e633-110">Return Type</span></span>|<span data-ttu-id="8e633-111">说明</span><span class="sxs-lookup"><span data-stu-id="8e633-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8e633-112">列出 organizations</span><span class="sxs-lookup"><span data-stu-id="8e633-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="8e633-113">[organization](../resources/intune-onboarding-organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8e633-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="8e633-114">列出 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8e633-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="8e633-115">获取 organization</span><span class="sxs-lookup"><span data-stu-id="8e633-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="8e633-116">organization</span><span class="sxs-lookup"><span data-stu-id="8e633-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="8e633-117">读取 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8e633-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="8e633-118">更新 organization</span><span class="sxs-lookup"><span data-stu-id="8e633-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="8e633-119">organization</span><span class="sxs-lookup"><span data-stu-id="8e633-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="8e633-120">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8e633-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="8e633-121">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="8e633-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="8e633-122">Int32</span><span class="sxs-lookup"><span data-stu-id="8e633-122">Int32</span></span>|<span data-ttu-id="8e633-123">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="8e633-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="8e633-124">属性</span><span class="sxs-lookup"><span data-stu-id="8e633-124">Properties</span></span>
|<span data-ttu-id="8e633-125">属性</span><span class="sxs-lookup"><span data-stu-id="8e633-125">Property</span></span>|<span data-ttu-id="8e633-126">类型</span><span class="sxs-lookup"><span data-stu-id="8e633-126">Type</span></span>|<span data-ttu-id="8e633-127">说明</span><span class="sxs-lookup"><span data-stu-id="8e633-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e633-128">id</span><span class="sxs-lookup"><span data-stu-id="8e633-128">id</span></span>|<span data-ttu-id="8e633-129">String</span><span class="sxs-lookup"><span data-stu-id="8e633-129">String</span></span>|<span data-ttu-id="8e633-130">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="8e633-130">The GUID for the object.</span></span>|
|<span data-ttu-id="8e633-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="8e633-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="8e633-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="8e633-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="8e633-133">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="8e633-133">Mobile device management authority.</span></span> <span data-ttu-id="8e633-134">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="8e633-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="8e633-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="8e633-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="8e633-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="8e633-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="8e633-137">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="8e633-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e633-138">关系</span><span class="sxs-lookup"><span data-stu-id="8e633-138">Relationships</span></span>
<span data-ttu-id="8e633-139">无</span><span class="sxs-lookup"><span data-stu-id="8e633-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e633-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e633-140">JSON Representation</span></span>
<span data-ttu-id="8e633-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e633-141">Here is a JSON representation of the resource.</span></span>
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




