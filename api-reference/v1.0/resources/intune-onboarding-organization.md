---
title: 组织资源类型
description: 组织资源表示在租户级别操作和配置的全局设置和资源的实例。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1e1afa1ded131844f687fa2dbad1a8e07639b264
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250052"
---
# <a name="organization-resource-type"></a><span data-ttu-id="4827a-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="4827a-103">organization resource type</span></span>

> <span data-ttu-id="4827a-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4827a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4827a-105">组织资源表示在租户级别操作和配置的全局设置和资源的实例。</span><span class="sxs-lookup"><span data-stu-id="4827a-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="4827a-106">方法</span><span class="sxs-lookup"><span data-stu-id="4827a-106">Methods</span></span>
|<span data-ttu-id="4827a-107">方法</span><span class="sxs-lookup"><span data-stu-id="4827a-107">Method</span></span>|<span data-ttu-id="4827a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4827a-108">Return Type</span></span>|<span data-ttu-id="4827a-109">说明</span><span class="sxs-lookup"><span data-stu-id="4827a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4827a-110">列出 organizations</span><span class="sxs-lookup"><span data-stu-id="4827a-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="4827a-111">[organization](../resources/intune-onboarding-organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4827a-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="4827a-112">列出 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4827a-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="4827a-113">获取 organization</span><span class="sxs-lookup"><span data-stu-id="4827a-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="4827a-114">组织</span><span class="sxs-lookup"><span data-stu-id="4827a-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="4827a-115">读取 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4827a-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="4827a-116">更新 organization</span><span class="sxs-lookup"><span data-stu-id="4827a-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="4827a-117">organization</span><span class="sxs-lookup"><span data-stu-id="4827a-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="4827a-118">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4827a-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="4827a-119">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="4827a-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="4827a-120">Int32</span><span class="sxs-lookup"><span data-stu-id="4827a-120">Int32</span></span>|<span data-ttu-id="4827a-121">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="4827a-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="4827a-122">属性</span><span class="sxs-lookup"><span data-stu-id="4827a-122">Properties</span></span>
|<span data-ttu-id="4827a-123">属性</span><span class="sxs-lookup"><span data-stu-id="4827a-123">Property</span></span>|<span data-ttu-id="4827a-124">类型</span><span class="sxs-lookup"><span data-stu-id="4827a-124">Type</span></span>|<span data-ttu-id="4827a-125">说明</span><span class="sxs-lookup"><span data-stu-id="4827a-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4827a-126">id</span><span class="sxs-lookup"><span data-stu-id="4827a-126">id</span></span>|<span data-ttu-id="4827a-127">String</span><span class="sxs-lookup"><span data-stu-id="4827a-127">String</span></span>|<span data-ttu-id="4827a-128">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="4827a-128">The GUID for the object.</span></span>|
|<span data-ttu-id="4827a-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="4827a-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="4827a-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="4827a-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="4827a-131">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="4827a-131">Mobile device management authority.</span></span> <span data-ttu-id="4827a-132">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="4827a-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4827a-133">Relationships</span><span class="sxs-lookup"><span data-stu-id="4827a-133">Relationships</span></span>
<span data-ttu-id="4827a-134">无</span><span class="sxs-lookup"><span data-stu-id="4827a-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4827a-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4827a-135">JSON Representation</span></span>
<span data-ttu-id="4827a-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4827a-136">Here is a JSON representation of the resource.</span></span>
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
  "mobileDeviceManagementAuthority": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [

"Warning: Resource microsoft.graph.organization is defined in multiple files: /api-reference/v1.0/resources/intune_onboarding_organization.md, /api-reference/v1.0/resources/organization.md",

"Warning: Schema type organization has a different BaseType value microsoft.graph.directoryObject than the documentation .",

"Warning: Schema type organization has a different OpenType value False than the documentation True.",

"Warning: Resource organization has multiple declarations with mismatched OpenType declarations."

  ],

}
-->



