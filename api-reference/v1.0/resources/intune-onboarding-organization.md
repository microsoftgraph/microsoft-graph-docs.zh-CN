---
title: 组织资源类型
description: 组织资源表示在租户级别操作和配置的全局设置和资源的实例。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd38274fea11f4312b60719fe04464d9b283fe9c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961371"
---
# <a name="organization-resource-type"></a><span data-ttu-id="c6fe7-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="c6fe7-103">organization resource type</span></span>

> <span data-ttu-id="c6fe7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c6fe7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6fe7-105">组织资源表示在租户级别操作和配置的全局设置和资源的实例。</span><span class="sxs-lookup"><span data-stu-id="c6fe7-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="c6fe7-106">方法</span><span class="sxs-lookup"><span data-stu-id="c6fe7-106">Methods</span></span>
|<span data-ttu-id="c6fe7-107">方法</span><span class="sxs-lookup"><span data-stu-id="c6fe7-107">Method</span></span>|<span data-ttu-id="c6fe7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c6fe7-108">Return Type</span></span>|<span data-ttu-id="c6fe7-109">说明</span><span class="sxs-lookup"><span data-stu-id="c6fe7-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6fe7-110">列出 organizations</span><span class="sxs-lookup"><span data-stu-id="c6fe7-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="c6fe7-111">[organization](../resources/intune-onboarding-organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c6fe7-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="c6fe7-112">列出 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6fe7-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="c6fe7-113">获取 organization</span><span class="sxs-lookup"><span data-stu-id="c6fe7-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="c6fe7-114">organization</span><span class="sxs-lookup"><span data-stu-id="c6fe7-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="c6fe7-115">读取 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c6fe7-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="c6fe7-116">更新 organization</span><span class="sxs-lookup"><span data-stu-id="c6fe7-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="c6fe7-117">organization</span><span class="sxs-lookup"><span data-stu-id="c6fe7-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="c6fe7-118">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c6fe7-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="c6fe7-119">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="c6fe7-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="c6fe7-120">Int32</span><span class="sxs-lookup"><span data-stu-id="c6fe7-120">Int32</span></span>|<span data-ttu-id="c6fe7-121">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="c6fe7-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="c6fe7-122">属性</span><span class="sxs-lookup"><span data-stu-id="c6fe7-122">Properties</span></span>
|<span data-ttu-id="c6fe7-123">属性</span><span class="sxs-lookup"><span data-stu-id="c6fe7-123">Property</span></span>|<span data-ttu-id="c6fe7-124">类型</span><span class="sxs-lookup"><span data-stu-id="c6fe7-124">Type</span></span>|<span data-ttu-id="c6fe7-125">说明</span><span class="sxs-lookup"><span data-stu-id="c6fe7-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6fe7-126">id</span><span class="sxs-lookup"><span data-stu-id="c6fe7-126">id</span></span>|<span data-ttu-id="c6fe7-127">String</span><span class="sxs-lookup"><span data-stu-id="c6fe7-127">String</span></span>|<span data-ttu-id="c6fe7-128">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="c6fe7-128">The GUID for the object.</span></span>|
|<span data-ttu-id="c6fe7-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="c6fe7-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="c6fe7-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="c6fe7-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="c6fe7-131">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="c6fe7-131">Mobile device management authority.</span></span> <span data-ttu-id="c6fe7-132">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="c6fe7-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6fe7-133">Relationships</span><span class="sxs-lookup"><span data-stu-id="c6fe7-133">Relationships</span></span>
<span data-ttu-id="c6fe7-134">无</span><span class="sxs-lookup"><span data-stu-id="c6fe7-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c6fe7-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6fe7-135">JSON Representation</span></span>
<span data-ttu-id="c6fe7-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6fe7-136">Here is a JSON representation of the resource.</span></span>
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

