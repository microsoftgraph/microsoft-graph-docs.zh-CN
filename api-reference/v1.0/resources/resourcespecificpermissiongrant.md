---
title: resourceSpecificPermissionGrant 资源类型
description: 指定特定 Azure AD 应用具有的权限。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2fd6e9e09a092719f20de2c34f2120537cd00606
ms.sourcegitcommit: b5fbb1a715e3479bdd095ef00deb0c932eafc328
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2021
ms.locfileid: "53162194"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="e4470-103">resourceSpecificPermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4470-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="e4470-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4470-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e4470-105">resourceSpecificPermissionGrant 声明已授予特定 AzureAD 应用的权限，该权限适用于 Microsoft Graph 中的资源实例。</span><span class="sxs-lookup"><span data-stu-id="e4470-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

<span data-ttu-id="e4470-106">有关授予应用同意访问资源的特定实例的权限，请参阅特定于 [资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。</span><span class="sxs-lookup"><span data-stu-id="e4470-106">For more information about granting apps consent to access a specific instance of a resource, see [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

## <a name="methods"></a><span data-ttu-id="e4470-107">方法</span><span class="sxs-lookup"><span data-stu-id="e4470-107">Methods</span></span>

|  <span data-ttu-id="e4470-108">方法</span><span class="sxs-lookup"><span data-stu-id="e4470-108">Method</span></span>                                                                   |  <span data-ttu-id="e4470-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e4470-109">Return Type</span></span>                                                                     | <span data-ttu-id="e4470-110">说明</span><span class="sxs-lookup"><span data-stu-id="e4470-110">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="e4470-111">列出组的权限管理</span><span class="sxs-lookup"><span data-stu-id="e4470-111">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="e4470-112">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e4470-112">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="e4470-113">列出特定组中已授予的资源特定 [权限](group.md)。</span><span class="sxs-lookup"><span data-stu-id="e4470-113">List resource-specific permissions that have been granted in a specific [group](group.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="e4470-114">属性</span><span class="sxs-lookup"><span data-stu-id="e4470-114">Properties</span></span>

| <span data-ttu-id="e4470-115">属性</span><span class="sxs-lookup"><span data-stu-id="e4470-115">Property</span></span>        | <span data-ttu-id="e4470-116">类型</span><span class="sxs-lookup"><span data-stu-id="e4470-116">Type</span></span>          | <span data-ttu-id="e4470-117">说明</span><span class="sxs-lookup"><span data-stu-id="e4470-117">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="e4470-118">id</span><span class="sxs-lookup"><span data-stu-id="e4470-118">id</span></span>              | <span data-ttu-id="e4470-119">string</span><span class="sxs-lookup"><span data-stu-id="e4470-119">string</span></span>        | <span data-ttu-id="e4470-120">特定于资源的权限授予的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e4470-120">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="e4470-121">只读。</span><span class="sxs-lookup"><span data-stu-id="e4470-121">Read-only.</span></span>           |
| <span data-ttu-id="e4470-122">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4470-122">deletedDateTime</span></span> | <span data-ttu-id="e4470-123">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4470-123">dateTimeOffset</span></span>| <span data-ttu-id="e4470-124">未使用。</span><span class="sxs-lookup"><span data-stu-id="e4470-124">Not used.</span></span>                                                                             |
| <span data-ttu-id="e4470-125">clientId</span><span class="sxs-lookup"><span data-stu-id="e4470-125">clientId</span></span>        | <span data-ttu-id="e4470-126">字符串</span><span class="sxs-lookup"><span data-stu-id="e4470-126">string</span></span>        | <span data-ttu-id="e4470-127">已授予访问权限的 Azure AD 应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="e4470-127">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="e4470-128">只读。</span><span class="sxs-lookup"><span data-stu-id="e4470-128">Read-only.</span></span>                            |
| <span data-ttu-id="e4470-129">clientAppId</span><span class="sxs-lookup"><span data-stu-id="e4470-129">clientAppId</span></span>     | <span data-ttu-id="e4470-130">字符串</span><span class="sxs-lookup"><span data-stu-id="e4470-130">string</span></span>        | <span data-ttu-id="e4470-131">已授予访问权限的 Azure AD 应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="e4470-131">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="e4470-132">只读。</span><span class="sxs-lookup"><span data-stu-id="e4470-132">Read-only.</span></span>   |
| <span data-ttu-id="e4470-133">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="e4470-133">resourceAppId</span></span>   | <span data-ttu-id="e4470-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e4470-134">string</span></span>        | <span data-ttu-id="e4470-135">托管资源的 Azure AD 应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="e4470-135">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="e4470-136">只读。</span><span class="sxs-lookup"><span data-stu-id="e4470-136">Read-only.</span></span>                        |
| <span data-ttu-id="e4470-137">permissionType</span><span class="sxs-lookup"><span data-stu-id="e4470-137">permissionType</span></span>  | <span data-ttu-id="e4470-138">字符串</span><span class="sxs-lookup"><span data-stu-id="e4470-138">string</span></span>        | <span data-ttu-id="e4470-139">权限的类型。</span><span class="sxs-lookup"><span data-stu-id="e4470-139">The type of permission.</span></span> <span data-ttu-id="e4470-140">可能的值是：`Application`、`Delegated`。</span><span class="sxs-lookup"><span data-stu-id="e4470-140">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="e4470-141">只读。</span><span class="sxs-lookup"><span data-stu-id="e4470-141">Read-only.</span></span> |
| <span data-ttu-id="e4470-142">permission</span><span class="sxs-lookup"><span data-stu-id="e4470-142">permission</span></span>      | <span data-ttu-id="e4470-143">字符串</span><span class="sxs-lookup"><span data-stu-id="e4470-143">string</span></span>        | <span data-ttu-id="e4470-144">特定于资源的权限的名称。</span><span class="sxs-lookup"><span data-stu-id="e4470-144">The name of the resource-specific permission.</span></span> <span data-ttu-id="e4470-145">只读。</span><span class="sxs-lookup"><span data-stu-id="e4470-145">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="e4470-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4470-146">JSON representation</span></span>

<span data-ttu-id="e4470-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4470-147">The following is a JSON representation of the resource.</span></span>

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