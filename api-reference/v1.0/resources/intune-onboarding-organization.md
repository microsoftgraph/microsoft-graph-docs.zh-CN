---
title: 组织资源类型
description: 组织资源表示在租户级别操作和配置的全局设置和资源的实例。
author: tfitzmac
ms.openlocfilehash: da2d127dc5ba44187d8a3a066f5fe261d3dee859
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322846"
---
# <a name="organization-resource-type"></a><span data-ttu-id="f93c6-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="f93c6-103">organization resource type</span></span>

> <span data-ttu-id="f93c6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f93c6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f93c6-105">组织资源表示在租户级别操作和配置的全局设置和资源的实例。</span><span class="sxs-lookup"><span data-stu-id="f93c6-105">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>
## <a name="methods"></a><span data-ttu-id="f93c6-106">方法</span><span class="sxs-lookup"><span data-stu-id="f93c6-106">Methods</span></span>
|<span data-ttu-id="f93c6-107">方法</span><span class="sxs-lookup"><span data-stu-id="f93c6-107">Method</span></span>|<span data-ttu-id="f93c6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f93c6-108">Return Type</span></span>|<span data-ttu-id="f93c6-109">说明</span><span class="sxs-lookup"><span data-stu-id="f93c6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f93c6-110">列出 organizations</span><span class="sxs-lookup"><span data-stu-id="f93c6-110">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="f93c6-111">[organization](../resources/intune-onboarding-organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f93c6-111">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="f93c6-112">列出 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f93c6-112">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="f93c6-113">获取 organization</span><span class="sxs-lookup"><span data-stu-id="f93c6-113">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="f93c6-114">organization</span><span class="sxs-lookup"><span data-stu-id="f93c6-114">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="f93c6-115">读取 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f93c6-115">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="f93c6-116">更新 organization</span><span class="sxs-lookup"><span data-stu-id="f93c6-116">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="f93c6-117">organization</span><span class="sxs-lookup"><span data-stu-id="f93c6-117">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="f93c6-118">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f93c6-118">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="f93c6-119">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="f93c6-119">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="f93c6-120">Int32</span><span class="sxs-lookup"><span data-stu-id="f93c6-120">Int32</span></span>|<span data-ttu-id="f93c6-121">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="f93c6-121">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="f93c6-122">属性</span><span class="sxs-lookup"><span data-stu-id="f93c6-122">Properties</span></span>
|<span data-ttu-id="f93c6-123">属性</span><span class="sxs-lookup"><span data-stu-id="f93c6-123">Property</span></span>|<span data-ttu-id="f93c6-124">类型</span><span class="sxs-lookup"><span data-stu-id="f93c6-124">Type</span></span>|<span data-ttu-id="f93c6-125">说明</span><span class="sxs-lookup"><span data-stu-id="f93c6-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f93c6-126">id</span><span class="sxs-lookup"><span data-stu-id="f93c6-126">id</span></span>|<span data-ttu-id="f93c6-127">String</span><span class="sxs-lookup"><span data-stu-id="f93c6-127">String</span></span>|<span data-ttu-id="f93c6-128">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="f93c6-128">The GUID for the object.</span></span>|
|<span data-ttu-id="f93c6-129">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="f93c6-129">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="f93c6-130">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="f93c6-130">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="f93c6-131">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="f93c6-131">Mobile device management authority.</span></span> <span data-ttu-id="f93c6-132">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="f93c6-132">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f93c6-133">Relationships</span><span class="sxs-lookup"><span data-stu-id="f93c6-133">Relationships</span></span>
<span data-ttu-id="f93c6-134">无</span><span class="sxs-lookup"><span data-stu-id="f93c6-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f93c6-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f93c6-135">JSON Representation</span></span>
<span data-ttu-id="f93c6-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f93c6-136">Here is a JSON representation of the resource.</span></span>
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

