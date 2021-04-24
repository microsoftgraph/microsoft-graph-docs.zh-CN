---
title: resourceSpecificPermissionGrant 资源类型
description: 指定特定 Azure AD 应用具有的权限。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 769c4d405473ef800b92fbecb8797588cf59eb57
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944289"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="e29f7-103">resourceSpecificPermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="e29f7-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="e29f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e29f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e29f7-105">resourceSpecificPermissionGrant 声明已授予特定 AzureAD 应用的权限，该权限适用于 Microsoft Graph 中的资源实例。</span><span class="sxs-lookup"><span data-stu-id="e29f7-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="e29f7-106">方法</span><span class="sxs-lookup"><span data-stu-id="e29f7-106">Methods</span></span>

|  <span data-ttu-id="e29f7-107">方法</span><span class="sxs-lookup"><span data-stu-id="e29f7-107">Method</span></span>                                                                   |  <span data-ttu-id="e29f7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e29f7-108">Return Type</span></span>                                                                     | <span data-ttu-id="e29f7-109">说明</span><span class="sxs-lookup"><span data-stu-id="e29f7-109">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="e29f7-110">列出组的权限授予</span><span class="sxs-lookup"><span data-stu-id="e29f7-110">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="e29f7-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e29f7-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="e29f7-112">列出特定组中已授予的权限。</span><span class="sxs-lookup"><span data-stu-id="e29f7-112">List permissions that have been granted in a specific group.</span></span> |

## <a name="properties"></a><span data-ttu-id="e29f7-113">属性</span><span class="sxs-lookup"><span data-stu-id="e29f7-113">Properties</span></span>

| <span data-ttu-id="e29f7-114">属性</span><span class="sxs-lookup"><span data-stu-id="e29f7-114">Property</span></span>        | <span data-ttu-id="e29f7-115">类型</span><span class="sxs-lookup"><span data-stu-id="e29f7-115">Type</span></span>          | <span data-ttu-id="e29f7-116">说明</span><span class="sxs-lookup"><span data-stu-id="e29f7-116">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="e29f7-117">id</span><span class="sxs-lookup"><span data-stu-id="e29f7-117">id</span></span>              | <span data-ttu-id="e29f7-118">string</span><span class="sxs-lookup"><span data-stu-id="e29f7-118">string</span></span>        | <span data-ttu-id="e29f7-119">特定于资源的权限授予的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e29f7-119">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="e29f7-120">只读。</span><span class="sxs-lookup"><span data-stu-id="e29f7-120">Read-only.</span></span>           |
| <span data-ttu-id="e29f7-121">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="e29f7-121">deletedDateTime</span></span> | <span data-ttu-id="e29f7-122">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e29f7-122">dateTimeOffset</span></span>| <span data-ttu-id="e29f7-123">未使用。</span><span class="sxs-lookup"><span data-stu-id="e29f7-123">Not used.</span></span>                                                                             |
| <span data-ttu-id="e29f7-124">clientId</span><span class="sxs-lookup"><span data-stu-id="e29f7-124">clientId</span></span>        | <span data-ttu-id="e29f7-125">string</span><span class="sxs-lookup"><span data-stu-id="e29f7-125">string</span></span>        | <span data-ttu-id="e29f7-126">已授予访问权限的 Azure AD 应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="e29f7-126">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="e29f7-127">只读。</span><span class="sxs-lookup"><span data-stu-id="e29f7-127">Read-only.</span></span>                            |
| <span data-ttu-id="e29f7-128">clientAppId</span><span class="sxs-lookup"><span data-stu-id="e29f7-128">clientAppId</span></span>     | <span data-ttu-id="e29f7-129">string</span><span class="sxs-lookup"><span data-stu-id="e29f7-129">string</span></span>        | <span data-ttu-id="e29f7-130">已授予访问权限的 Azure AD 应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="e29f7-130">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="e29f7-131">只读。</span><span class="sxs-lookup"><span data-stu-id="e29f7-131">Read-only.</span></span>   |
| <span data-ttu-id="e29f7-132">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="e29f7-132">resourceAppId</span></span>   | <span data-ttu-id="e29f7-133">string</span><span class="sxs-lookup"><span data-stu-id="e29f7-133">string</span></span>        | <span data-ttu-id="e29f7-134">托管资源的 Azure AD 应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="e29f7-134">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="e29f7-135">只读。</span><span class="sxs-lookup"><span data-stu-id="e29f7-135">Read-only.</span></span>                        |
| <span data-ttu-id="e29f7-136">permissionType</span><span class="sxs-lookup"><span data-stu-id="e29f7-136">permissionType</span></span>  | <span data-ttu-id="e29f7-137">string</span><span class="sxs-lookup"><span data-stu-id="e29f7-137">string</span></span>        | <span data-ttu-id="e29f7-138">权限的类型。</span><span class="sxs-lookup"><span data-stu-id="e29f7-138">The type of permission.</span></span> <span data-ttu-id="e29f7-139">可能的值是：`Application`、`Delegated`。</span><span class="sxs-lookup"><span data-stu-id="e29f7-139">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="e29f7-140">只读。</span><span class="sxs-lookup"><span data-stu-id="e29f7-140">Read-only.</span></span> |
| <span data-ttu-id="e29f7-141">permission</span><span class="sxs-lookup"><span data-stu-id="e29f7-141">permission</span></span>      | <span data-ttu-id="e29f7-142">string</span><span class="sxs-lookup"><span data-stu-id="e29f7-142">string</span></span>        | <span data-ttu-id="e29f7-143">权限的名称。</span><span class="sxs-lookup"><span data-stu-id="e29f7-143">The name of the permission.</span></span> <span data-ttu-id="e29f7-144">只读。</span><span class="sxs-lookup"><span data-stu-id="e29f7-144">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="e29f7-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e29f7-145">JSON representation</span></span>

<span data-ttu-id="e29f7-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e29f7-146">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.resourceSpecificPermissionGrant"
}-->

```json
{
  "id": "string (identifier)",
  "deletedDateTime": "dateTimeOffset",
  "clientId": "string",
  "clientAppId": "string",
  "resourceAppId": "string",
  "permissionType": "string",
  "permission": "string"
}
```