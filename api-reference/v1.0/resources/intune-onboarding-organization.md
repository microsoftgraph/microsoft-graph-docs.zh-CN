---
title: 组织资源类型
description: 组织资源表示在租户级别操作和配置的全局设置和资源的实例。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2af65c341f665fd358d03619a3cd3606723df123
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754949"
---
# <a name="organization-resource-type"></a><span data-ttu-id="cfd5c-103">组织资源类型</span><span class="sxs-lookup"><span data-stu-id="cfd5c-103">organization resource type</span></span>

<span data-ttu-id="cfd5c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfd5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cfd5c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cfd5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfd5c-106">组织资源表示在租户级别操作和配置的全局设置和资源的实例。</span><span class="sxs-lookup"><span data-stu-id="cfd5c-106">The organization resource represents an instance of global settings and resources which operate and are provisioned at the tenant-level.</span></span>

## <a name="methods"></a><span data-ttu-id="cfd5c-107">Methods</span><span class="sxs-lookup"><span data-stu-id="cfd5c-107">Methods</span></span>
|<span data-ttu-id="cfd5c-108">方法</span><span class="sxs-lookup"><span data-stu-id="cfd5c-108">Method</span></span>|<span data-ttu-id="cfd5c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="cfd5c-109">Return Type</span></span>|<span data-ttu-id="cfd5c-110">Description</span><span class="sxs-lookup"><span data-stu-id="cfd5c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cfd5c-111">列出 organizations</span><span class="sxs-lookup"><span data-stu-id="cfd5c-111">List organizations</span></span>](../api/intune-onboarding-organization-list.md)|<span data-ttu-id="cfd5c-112">[organization](../resources/intune-onboarding-organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cfd5c-112">[organization](../resources/intune-onboarding-organization.md) collection</span></span>|<span data-ttu-id="cfd5c-113">列出 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cfd5c-113">List properties and relationships of the [organization](../resources/intune-onboarding-organization.md) objects.</span></span>|
|[<span data-ttu-id="cfd5c-114">获取组织</span><span class="sxs-lookup"><span data-stu-id="cfd5c-114">Get organization</span></span>](../api/intune-onboarding-organization-get.md)|[<span data-ttu-id="cfd5c-115">组织</span><span class="sxs-lookup"><span data-stu-id="cfd5c-115">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="cfd5c-116">读取 [organization](../resources/intune-onboarding-organization.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cfd5c-116">Read properties and relationships of the [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="cfd5c-117">更新 organization</span><span class="sxs-lookup"><span data-stu-id="cfd5c-117">Update organization</span></span>](../api/intune-onboarding-organization-update.md)|[<span data-ttu-id="cfd5c-118">organization</span><span class="sxs-lookup"><span data-stu-id="cfd5c-118">organization</span></span>](../resources/intune-onboarding-organization.md)|<span data-ttu-id="cfd5c-119">更新 [organization](../resources/intune-onboarding-organization.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cfd5c-119">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>|
|[<span data-ttu-id="cfd5c-120">setMobileDeviceManagementAuthority 操作</span><span class="sxs-lookup"><span data-stu-id="cfd5c-120">setMobileDeviceManagementAuthority action</span></span>](../api/intune-onboarding-organization-setmobiledevicemanagementauthority.md)|<span data-ttu-id="cfd5c-121">Int32</span><span class="sxs-lookup"><span data-stu-id="cfd5c-121">Int32</span></span>|<span data-ttu-id="cfd5c-122">设置移动设备管理机构</span><span class="sxs-lookup"><span data-stu-id="cfd5c-122">Set mobile device management authority</span></span>|

## <a name="properties"></a><span data-ttu-id="cfd5c-123">属性</span><span class="sxs-lookup"><span data-stu-id="cfd5c-123">Properties</span></span>
|<span data-ttu-id="cfd5c-124">属性</span><span class="sxs-lookup"><span data-stu-id="cfd5c-124">Property</span></span>|<span data-ttu-id="cfd5c-125">类型</span><span class="sxs-lookup"><span data-stu-id="cfd5c-125">Type</span></span>|<span data-ttu-id="cfd5c-126">说明</span><span class="sxs-lookup"><span data-stu-id="cfd5c-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfd5c-127">id</span><span class="sxs-lookup"><span data-stu-id="cfd5c-127">id</span></span>|<span data-ttu-id="cfd5c-128">String</span><span class="sxs-lookup"><span data-stu-id="cfd5c-128">String</span></span>|<span data-ttu-id="cfd5c-129">对象的 GUID。</span><span class="sxs-lookup"><span data-stu-id="cfd5c-129">The GUID for the object.</span></span>|
|<span data-ttu-id="cfd5c-130">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="cfd5c-130">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="cfd5c-131">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="cfd5c-131">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="cfd5c-132">移动设备管理机构。</span><span class="sxs-lookup"><span data-stu-id="cfd5c-132">Mobile device management authority.</span></span> <span data-ttu-id="cfd5c-133">可取值为：`unknown`、`intune`、`sccm`、`office365`。</span><span class="sxs-lookup"><span data-stu-id="cfd5c-133">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cfd5c-134">关系</span><span class="sxs-lookup"><span data-stu-id="cfd5c-134">Relationships</span></span>
<span data-ttu-id="cfd5c-135">无</span><span class="sxs-lookup"><span data-stu-id="cfd5c-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfd5c-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cfd5c-136">JSON Representation</span></span>
<span data-ttu-id="cfd5c-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfd5c-137">Here is a JSON representation of the resource.</span></span>
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




