---
title: resourceSpecificPermissionGrant 资源类型
description: 指定特定 Azure AD 应用具有的权限。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f100d5658b2ecdc07daf928594180b0ce6129594
ms.sourcegitcommit: b5fbb1a715e3479bdd095ef00deb0c932eafc328
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2021
ms.locfileid: "53162218"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="432b5-103">resourceSpecificPermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="432b5-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="432b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="432b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="432b5-105">resourceSpecificPermissionGrant 声明已授予特定 AzureAD 应用的权限，该权限适用于 Microsoft Graph 中的资源实例。</span><span class="sxs-lookup"><span data-stu-id="432b5-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

<span data-ttu-id="432b5-106">有关授予应用同意访问资源的特定实例的权限，请参阅特定于 [资源的同意](/microsoftteams/platform/graph-api/rsc/resource-specific-consent)。</span><span class="sxs-lookup"><span data-stu-id="432b5-106">For more information about granting apps consent to access a specific instance of a resource, see [resource-specific consent](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).</span></span>

## <a name="methods"></a><span data-ttu-id="432b5-107">方法</span><span class="sxs-lookup"><span data-stu-id="432b5-107">Methods</span></span>

|  <span data-ttu-id="432b5-108">方法</span><span class="sxs-lookup"><span data-stu-id="432b5-108">Method</span></span>                                                                   |  <span data-ttu-id="432b5-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="432b5-109">Return Type</span></span>                                                                     | <span data-ttu-id="432b5-110">说明</span><span class="sxs-lookup"><span data-stu-id="432b5-110">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="432b5-111">列出聊天的权限管理</span><span class="sxs-lookup"><span data-stu-id="432b5-111">List permission grants of a chat</span></span>](../api/chat-list-permissiongrants.md)   | <span data-ttu-id="432b5-112">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="432b5-112">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="432b5-113">列出特定聊天中已授予的资源特定 [权限](chat.md)。</span><span class="sxs-lookup"><span data-stu-id="432b5-113">List resource-specific permissions that have been granted in a specific [chat](chat.md).</span></span>  |
|[<span data-ttu-id="432b5-114">列出组的权限管理</span><span class="sxs-lookup"><span data-stu-id="432b5-114">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="432b5-115">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="432b5-115">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="432b5-116">列出特定组中已授予的资源特定 [权限](group.md)。</span><span class="sxs-lookup"><span data-stu-id="432b5-116">List resource-specific permissions that have been granted in a specific [group](group.md).</span></span> |
|[<span data-ttu-id="432b5-117">列出团队的权限授予</span><span class="sxs-lookup"><span data-stu-id="432b5-117">List permission grants of a team</span></span>](../api/team-list-permissiongrants.md) | <span data-ttu-id="432b5-118">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="432b5-118">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="432b5-119">列出特定团队中已授予的资源特定 [权限](team.md)。</span><span class="sxs-lookup"><span data-stu-id="432b5-119">List resource-specific permissions that have been granted in a specific [team](team.md).</span></span> |

## <a name="properties"></a><span data-ttu-id="432b5-120">属性</span><span class="sxs-lookup"><span data-stu-id="432b5-120">Properties</span></span>

| <span data-ttu-id="432b5-121">属性</span><span class="sxs-lookup"><span data-stu-id="432b5-121">Property</span></span>        | <span data-ttu-id="432b5-122">类型</span><span class="sxs-lookup"><span data-stu-id="432b5-122">Type</span></span>          | <span data-ttu-id="432b5-123">说明</span><span class="sxs-lookup"><span data-stu-id="432b5-123">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="432b5-124">id</span><span class="sxs-lookup"><span data-stu-id="432b5-124">id</span></span>              | <span data-ttu-id="432b5-125">string</span><span class="sxs-lookup"><span data-stu-id="432b5-125">string</span></span>        | <span data-ttu-id="432b5-126">特定于资源的权限授予的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="432b5-126">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="432b5-127">只读。</span><span class="sxs-lookup"><span data-stu-id="432b5-127">Read-only.</span></span>           |
| <span data-ttu-id="432b5-128">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="432b5-128">deletedDateTime</span></span> | <span data-ttu-id="432b5-129">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="432b5-129">dateTimeOffset</span></span>| <span data-ttu-id="432b5-130">未使用。</span><span class="sxs-lookup"><span data-stu-id="432b5-130">Not used.</span></span>                                                                             |
| <span data-ttu-id="432b5-131">clientId</span><span class="sxs-lookup"><span data-stu-id="432b5-131">clientId</span></span>        | <span data-ttu-id="432b5-132">string</span><span class="sxs-lookup"><span data-stu-id="432b5-132">string</span></span>        | <span data-ttu-id="432b5-133">已授予访问权限的 Azure AD 应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="432b5-133">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="432b5-134">只读。</span><span class="sxs-lookup"><span data-stu-id="432b5-134">Read-only.</span></span>                            |
| <span data-ttu-id="432b5-135">clientAppId</span><span class="sxs-lookup"><span data-stu-id="432b5-135">clientAppId</span></span>     | <span data-ttu-id="432b5-136">string</span><span class="sxs-lookup"><span data-stu-id="432b5-136">string</span></span>        | <span data-ttu-id="432b5-137">已授予访问权限的 Azure AD 应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="432b5-137">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="432b5-138">只读。</span><span class="sxs-lookup"><span data-stu-id="432b5-138">Read-only.</span></span>   |
| <span data-ttu-id="432b5-139">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="432b5-139">resourceAppId</span></span>   | <span data-ttu-id="432b5-140">string</span><span class="sxs-lookup"><span data-stu-id="432b5-140">string</span></span>        | <span data-ttu-id="432b5-141">托管资源的 Azure AD 应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="432b5-141">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="432b5-142">只读。</span><span class="sxs-lookup"><span data-stu-id="432b5-142">Read-only.</span></span>                        |
| <span data-ttu-id="432b5-143">permissionType</span><span class="sxs-lookup"><span data-stu-id="432b5-143">permissionType</span></span>  | <span data-ttu-id="432b5-144">string</span><span class="sxs-lookup"><span data-stu-id="432b5-144">string</span></span>        | <span data-ttu-id="432b5-145">权限的类型。</span><span class="sxs-lookup"><span data-stu-id="432b5-145">The type of permission.</span></span> <span data-ttu-id="432b5-146">可能的值是：`Application`、`Delegated`。</span><span class="sxs-lookup"><span data-stu-id="432b5-146">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="432b5-147">只读。</span><span class="sxs-lookup"><span data-stu-id="432b5-147">Read-only.</span></span> |
| <span data-ttu-id="432b5-148">permission</span><span class="sxs-lookup"><span data-stu-id="432b5-148">permission</span></span>      | <span data-ttu-id="432b5-149">string</span><span class="sxs-lookup"><span data-stu-id="432b5-149">string</span></span>        | <span data-ttu-id="432b5-150">特定于资源的权限的名称。</span><span class="sxs-lookup"><span data-stu-id="432b5-150">The name of the resource-specific permission.</span></span> <span data-ttu-id="432b5-151">只读。</span><span class="sxs-lookup"><span data-stu-id="432b5-151">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="432b5-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="432b5-152">JSON representation</span></span>

<span data-ttu-id="432b5-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="432b5-153">The following is a JSON representation of the resource.</span></span>

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


