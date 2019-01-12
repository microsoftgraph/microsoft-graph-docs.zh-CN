---
title: 组织资源类型
description: 组织资源表示在租户级别操作和配置的全局设置和资源的实例。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8bc7a0fba8c5ecdc2b2a88062855e8b279721c45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990766"
---
# <a name="organization-resource-type"></a><span data-ttu-id="a7b46-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="a7b46-103">organization resource type</span></span>

> <span data-ttu-id="a7b46-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a7b46-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7b46-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a7b46-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7b46-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a7b46-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7b46-107">组织资源表示在租户级别操作和配置的全局设置和资源的实例。</span><span class="sxs-lookup"><span data-stu-id="a7b46-107">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="a7b46-108">方法</span><span class="sxs-lookup"><span data-stu-id="a7b46-108">Methods</span></span>
|<span data-ttu-id="a7b46-109">方法</span><span class="sxs-lookup"><span data-stu-id="a7b46-109">Method</span></span>|<span data-ttu-id="a7b46-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a7b46-110">Return Type</span></span>|<span data-ttu-id="a7b46-111">说明</span><span class="sxs-lookup"><span data-stu-id="a7b46-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7b46-112">列出 organizations</span><span class="sxs-lookup"><span data-stu-id="a7b46-112">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="a7b46-113">[organization](../resources/intune-onboarding-organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a7b46-113">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="a7b46-114">列出 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7b46-114">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="a7b46-115">获取 organization</span><span class="sxs-lookup"><span data-stu-id="a7b46-115">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="a7b46-116">organization</span><span class="sxs-lookup"><span data-stu-id="a7b46-116">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="a7b46-117">读取 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a7b46-117">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="a7b46-118">更新 organization</span><span class="sxs-lookup"><span data-stu-id="a7b46-118">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="a7b46-119">organization</span><span class="sxs-lookup"><span data-stu-id="a7b46-119">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="a7b46-120">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a7b46-120">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="a7b46-121">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="a7b46-121">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="a7b46-122">Int32</span><span class="sxs-lookup"><span data-stu-id="a7b46-122">Int32</span></span>|<span data-ttu-id="a7b46-123">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="a7b46-123">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="a7b46-124">属性</span><span class="sxs-lookup"><span data-stu-id="a7b46-124">Properties</span></span>
|<span data-ttu-id="a7b46-125">属性</span><span class="sxs-lookup"><span data-stu-id="a7b46-125">Property</span></span>|<span data-ttu-id="a7b46-126">类型</span><span class="sxs-lookup"><span data-stu-id="a7b46-126">Type</span></span>|<span data-ttu-id="a7b46-127">说明</span><span class="sxs-lookup"><span data-stu-id="a7b46-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7b46-128">id</span><span class="sxs-lookup"><span data-stu-id="a7b46-128">id</span></span>|<span data-ttu-id="a7b46-129">String</span><span class="sxs-lookup"><span data-stu-id="a7b46-129">String</span></span>|<span data-ttu-id="a7b46-130">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="a7b46-130">The GUID for the object.</span></span>|
|<span data-ttu-id="a7b46-131">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="a7b46-131">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="a7b46-132">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="a7b46-132">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="a7b46-133">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="a7b46-133">Mobile device management authority.</span></span> <span data-ttu-id="a7b46-134">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="a7b46-134">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|
|<span data-ttu-id="a7b46-135">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="a7b46-135">certificateConnectorSetting</span></span>|[<span data-ttu-id="a7b46-136">certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="a7b46-136">certificateConnectorSetting</span></span>](../resources/intune-onboarding-certificateconnectorsetting.md)|<span data-ttu-id="a7b46-137">证书连接器设置。</span><span class="sxs-lookup"><span data-stu-id="a7b46-137">Certificate connector setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7b46-138">Relationships</span><span class="sxs-lookup"><span data-stu-id="a7b46-138">Relationships</span></span>
<span data-ttu-id="a7b46-139">无</span><span class="sxs-lookup"><span data-stu-id="a7b46-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a7b46-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a7b46-140">JSON Representation</span></span>
<span data-ttu-id="a7b46-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a7b46-141">Here is a JSON representation of the resource.</span></span>
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





