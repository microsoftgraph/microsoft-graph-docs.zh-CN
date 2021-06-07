---
title: 用户资源类型
description: 表示 Azure Active Directory 用户对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b5f9c0ab08db3c8b9f6e48138e31d091ab5dde9a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755275"
---
# <a name="user-resource-type"></a><span data-ttu-id="92adf-103">用户资源类型</span><span class="sxs-lookup"><span data-stu-id="92adf-103">user resource type</span></span>

<span data-ttu-id="92adf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92adf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92adf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92adf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92adf-106">表示 Azure Active Directory 用户对象。</span><span class="sxs-lookup"><span data-stu-id="92adf-106">Represents an Azure Active Directory user object.</span></span>

## <a name="methods"></a><span data-ttu-id="92adf-107">方法</span><span class="sxs-lookup"><span data-stu-id="92adf-107">Methods</span></span>
|<span data-ttu-id="92adf-108">方法</span><span class="sxs-lookup"><span data-stu-id="92adf-108">Method</span></span>|<span data-ttu-id="92adf-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="92adf-109">Return Type</span></span>|<span data-ttu-id="92adf-110">说明</span><span class="sxs-lookup"><span data-stu-id="92adf-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="92adf-111">List users</span><span class="sxs-lookup"><span data-stu-id="92adf-111">List users</span></span>](../api/intune-mam-user-list.md)|<span data-ttu-id="92adf-112">[user](../resources/intune-mam-user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92adf-112">[user](../resources/intune-mam-user.md) collection</span></span>|<span data-ttu-id="92adf-113">列出 [user](../resources/intune-mam-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="92adf-113">List properties and relationships of the [user](../resources/intune-mam-user.md) objects.</span></span>|
|[<span data-ttu-id="92adf-114">Get user</span><span class="sxs-lookup"><span data-stu-id="92adf-114">Get user</span></span>](../api/intune-mam-user-get.md)|[<span data-ttu-id="92adf-115">user</span><span class="sxs-lookup"><span data-stu-id="92adf-115">user</span></span>](../resources/intune-mam-user.md)|<span data-ttu-id="92adf-116">读取 [user](../resources/intune-mam-user.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="92adf-116">Read properties and relationships of the [user](../resources/intune-mam-user.md) object.</span></span>|
|[<span data-ttu-id="92adf-117">Create user</span><span class="sxs-lookup"><span data-stu-id="92adf-117">Create user</span></span>](../api/intune-mam-user-create.md)|[<span data-ttu-id="92adf-118">user</span><span class="sxs-lookup"><span data-stu-id="92adf-118">user</span></span>](../resources/intune-mam-user.md)|<span data-ttu-id="92adf-119">创建新的 [user](../resources/intune-mam-user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="92adf-119">Create a new [user](../resources/intune-mam-user.md) object.</span></span>|
|[<span data-ttu-id="92adf-120">Delete user</span><span class="sxs-lookup"><span data-stu-id="92adf-120">Delete user</span></span>](../api/intune-mam-user-delete.md)|<span data-ttu-id="92adf-121">None</span><span class="sxs-lookup"><span data-stu-id="92adf-121">None</span></span>|<span data-ttu-id="92adf-122">删除 [user](../resources/intune-mam-user.md)。</span><span class="sxs-lookup"><span data-stu-id="92adf-122">Deletes a [user](../resources/intune-mam-user.md).</span></span>|
|[<span data-ttu-id="92adf-123">Update user</span><span class="sxs-lookup"><span data-stu-id="92adf-123">Update user</span></span>](../api/intune-mam-user-update.md)|[<span data-ttu-id="92adf-124">user</span><span class="sxs-lookup"><span data-stu-id="92adf-124">user</span></span>](../resources/intune-mam-user.md)|<span data-ttu-id="92adf-125">更新 [user](../resources/intune-mam-user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="92adf-125">Update the properties of a [user](../resources/intune-mam-user.md) object.</span></span>|
|[<span data-ttu-id="92adf-126">getManagedAppDiagnosticStatuses 函数</span><span class="sxs-lookup"><span data-stu-id="92adf-126">getManagedAppDiagnosticStatuses function</span></span>](../api/intune-mam-user-getmanagedappdiagnosticstatuses.md)|<span data-ttu-id="92adf-127">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92adf-127">[managedAppDiagnosticStatus](../resources/intune-mam-managedappdiagnosticstatus.md) collection</span></span>|<span data-ttu-id="92adf-128">获取给定用户的诊断验证状态。</span><span class="sxs-lookup"><span data-stu-id="92adf-128">Gets diagnostics validation status for a given user.</span></span>|
|[<span data-ttu-id="92adf-129">getManagedAppPolicies 函数</span><span class="sxs-lookup"><span data-stu-id="92adf-129">getManagedAppPolicies function</span></span>](../api/intune-mam-user-getmanagedapppolicies.md)|<span data-ttu-id="92adf-130">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92adf-130">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="92adf-131">获取给定用户的应用限制。</span><span class="sxs-lookup"><span data-stu-id="92adf-131">Gets app restrictions for a given user.</span></span>|
|[<span data-ttu-id="92adf-132">wipeManagedAppRegistrationsByDeviceTag 操作</span><span class="sxs-lookup"><span data-stu-id="92adf-132">wipeManagedAppRegistrationsByDeviceTag action</span></span>](../api/intune-mam-user-wipemanagedappregistrationsbydevicetag.md)|<span data-ttu-id="92adf-133">无</span><span class="sxs-lookup"><span data-stu-id="92adf-133">None</span></span>|<span data-ttu-id="92adf-134">对含有指定设备标记的应用注册发布擦除操作。</span><span class="sxs-lookup"><span data-stu-id="92adf-134">Issues a wipe operation on an app registration with specified device tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="92adf-135">属性</span><span class="sxs-lookup"><span data-stu-id="92adf-135">Properties</span></span>
|<span data-ttu-id="92adf-136">属性</span><span class="sxs-lookup"><span data-stu-id="92adf-136">Property</span></span>|<span data-ttu-id="92adf-137">类型</span><span class="sxs-lookup"><span data-stu-id="92adf-137">Type</span></span>|<span data-ttu-id="92adf-138">说明</span><span class="sxs-lookup"><span data-stu-id="92adf-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92adf-139">id</span><span class="sxs-lookup"><span data-stu-id="92adf-139">id</span></span>|<span data-ttu-id="92adf-140">String</span><span class="sxs-lookup"><span data-stu-id="92adf-140">String</span></span>|<span data-ttu-id="92adf-141">用户标识符。</span><span class="sxs-lookup"><span data-stu-id="92adf-141">The user identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="92adf-142">关系</span><span class="sxs-lookup"><span data-stu-id="92adf-142">Relationships</span></span>
|<span data-ttu-id="92adf-143">关系</span><span class="sxs-lookup"><span data-stu-id="92adf-143">Relationship</span></span>|<span data-ttu-id="92adf-144">类型</span><span class="sxs-lookup"><span data-stu-id="92adf-144">Type</span></span>|<span data-ttu-id="92adf-145">说明</span><span class="sxs-lookup"><span data-stu-id="92adf-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92adf-146">managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="92adf-146">managedAppRegistrations</span></span>|<span data-ttu-id="92adf-147">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="92adf-147">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="92adf-148">属于用户的零个或多个托管的应用注册。</span><span class="sxs-lookup"><span data-stu-id="92adf-148">Zero or more managed app registrations that belong to the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92adf-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92adf-149">JSON Representation</span></span>
<span data-ttu-id="92adf-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92adf-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```




