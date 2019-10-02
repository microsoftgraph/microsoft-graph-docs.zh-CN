---
title: 组织资源类型
description: 组织资源表示在租户级别操作和配置的全局设置和资源的实例。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 258e3683b988aa914cd43f2748a07032d72c08e9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360739"
---
# <a name="organization-resource-type"></a><span data-ttu-id="39418-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="39418-103">organization resource type</span></span>

> <span data-ttu-id="39418-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="39418-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39418-105">组织资源表示在租户级别操作和配置的全局设置和资源的实例。</span><span class="sxs-lookup"><span data-stu-id="39418-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="39418-106">方法</span><span class="sxs-lookup"><span data-stu-id="39418-106">Methods</span></span>
|<span data-ttu-id="39418-107">方法</span><span class="sxs-lookup"><span data-stu-id="39418-107">Method</span></span>|<span data-ttu-id="39418-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="39418-108">Return Type</span></span>|<span data-ttu-id="39418-109">说明</span><span class="sxs-lookup"><span data-stu-id="39418-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39418-110">列出 organizations</span><span class="sxs-lookup"><span data-stu-id="39418-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="39418-111">[organization](../resources/intune-onboarding-organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39418-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="39418-112">列出 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39418-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="39418-113">获取组织</span><span class="sxs-lookup"><span data-stu-id="39418-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="39418-114">组织</span><span class="sxs-lookup"><span data-stu-id="39418-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="39418-115">读取 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="39418-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="39418-116">更新 organization</span><span class="sxs-lookup"><span data-stu-id="39418-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="39418-117">organization</span><span class="sxs-lookup"><span data-stu-id="39418-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="39418-118">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="39418-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="39418-119">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="39418-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="39418-120">Int32</span><span class="sxs-lookup"><span data-stu-id="39418-120">Int32</span></span>|<span data-ttu-id="39418-121">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="39418-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="39418-122">属性</span><span class="sxs-lookup"><span data-stu-id="39418-122">Properties</span></span>
|<span data-ttu-id="39418-123">属性</span><span class="sxs-lookup"><span data-stu-id="39418-123">Property</span></span>|<span data-ttu-id="39418-124">类型</span><span class="sxs-lookup"><span data-stu-id="39418-124">Type</span></span>|<span data-ttu-id="39418-125">说明</span><span class="sxs-lookup"><span data-stu-id="39418-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39418-126">id</span><span class="sxs-lookup"><span data-stu-id="39418-126">id</span></span>|<span data-ttu-id="39418-127">String</span><span class="sxs-lookup"><span data-stu-id="39418-127">String</span></span>|<span data-ttu-id="39418-128">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="39418-128">The GUID for the object.</span></span>|
|<span data-ttu-id="39418-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="39418-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="39418-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="39418-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="39418-131">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="39418-131">Mobile device management authority.</span></span> <span data-ttu-id="39418-132">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="39418-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39418-133">关系</span><span class="sxs-lookup"><span data-stu-id="39418-133">Relationships</span></span>
<span data-ttu-id="39418-134">无</span><span class="sxs-lookup"><span data-stu-id="39418-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39418-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39418-135">JSON Representation</span></span>
<span data-ttu-id="39418-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39418-136">Here is a JSON representation of the resource.</span></span>
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




