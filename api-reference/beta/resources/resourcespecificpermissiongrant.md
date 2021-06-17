---
title: resourceSpecificPermissionGrant 资源类型
description: 指定特定 Azure AD 应用具有的权限。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 56d7ea203f4ed72f45a3650197c1484f817567e6
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992308"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="9c15a-103">resourceSpecificPermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="9c15a-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="9c15a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c15a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c15a-105">resourceSpecificPermissionGrant 声明已授予特定 AzureAD 应用的权限，该权限适用于 Microsoft Graph 中的资源实例。</span><span class="sxs-lookup"><span data-stu-id="9c15a-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="9c15a-106">方法</span><span class="sxs-lookup"><span data-stu-id="9c15a-106">Methods</span></span>

|  <span data-ttu-id="9c15a-107">方法</span><span class="sxs-lookup"><span data-stu-id="9c15a-107">Method</span></span>                                                                   |  <span data-ttu-id="9c15a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9c15a-108">Return Type</span></span>                                                                     | <span data-ttu-id="9c15a-109">说明</span><span class="sxs-lookup"><span data-stu-id="9c15a-109">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="9c15a-110">聊天的列表权限授予</span><span class="sxs-lookup"><span data-stu-id="9c15a-110">List permission grants of a chat</span></span>](../api/chat-list-permissiongrants.md)   | <span data-ttu-id="9c15a-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9c15a-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="9c15a-112">列出特定聊天中已授予的权限。</span><span class="sxs-lookup"><span data-stu-id="9c15a-112">List permissions that have been granted in a specific chat.</span></span>  |
|[<span data-ttu-id="9c15a-113">列出组的权限授予</span><span class="sxs-lookup"><span data-stu-id="9c15a-113">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="9c15a-114">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9c15a-114">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="9c15a-115">列出特定组中已授予的权限。</span><span class="sxs-lookup"><span data-stu-id="9c15a-115">List permissions that have been granted in a specific group.</span></span> |
|[<span data-ttu-id="9c15a-116">列出团队的权限授予</span><span class="sxs-lookup"><span data-stu-id="9c15a-116">List permission grants of a team</span></span>](../api/team-list-permissiongrants.md)   | <span data-ttu-id="9c15a-117">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9c15a-117">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="9c15a-118">列出特定团队已授予的权限。</span><span class="sxs-lookup"><span data-stu-id="9c15a-118">List permissions that have been granted in a specific team.</span></span>  |

## <a name="properties"></a><span data-ttu-id="9c15a-119">属性</span><span class="sxs-lookup"><span data-stu-id="9c15a-119">Properties</span></span>

| <span data-ttu-id="9c15a-120">属性</span><span class="sxs-lookup"><span data-stu-id="9c15a-120">Property</span></span>        | <span data-ttu-id="9c15a-121">类型</span><span class="sxs-lookup"><span data-stu-id="9c15a-121">Type</span></span>          | <span data-ttu-id="9c15a-122">说明</span><span class="sxs-lookup"><span data-stu-id="9c15a-122">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="9c15a-123">id</span><span class="sxs-lookup"><span data-stu-id="9c15a-123">id</span></span>              | <span data-ttu-id="9c15a-124">string</span><span class="sxs-lookup"><span data-stu-id="9c15a-124">string</span></span>        | <span data-ttu-id="9c15a-125">特定于资源的权限授予的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9c15a-125">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="9c15a-126">只读。</span><span class="sxs-lookup"><span data-stu-id="9c15a-126">Read-only.</span></span>           |
| <span data-ttu-id="9c15a-127">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c15a-127">deletedDateTime</span></span> | <span data-ttu-id="9c15a-128">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c15a-128">dateTimeOffset</span></span>| <span data-ttu-id="9c15a-129">未使用。</span><span class="sxs-lookup"><span data-stu-id="9c15a-129">Not used.</span></span>                                                                             |
| <span data-ttu-id="9c15a-130">clientId</span><span class="sxs-lookup"><span data-stu-id="9c15a-130">clientId</span></span>        | <span data-ttu-id="9c15a-131">string</span><span class="sxs-lookup"><span data-stu-id="9c15a-131">string</span></span>        | <span data-ttu-id="9c15a-132">已授予访问权限的 Azure AD 应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="9c15a-132">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="9c15a-133">只读。</span><span class="sxs-lookup"><span data-stu-id="9c15a-133">Read-only.</span></span>                            |
| <span data-ttu-id="9c15a-134">clientAppId</span><span class="sxs-lookup"><span data-stu-id="9c15a-134">clientAppId</span></span>     | <span data-ttu-id="9c15a-135">string</span><span class="sxs-lookup"><span data-stu-id="9c15a-135">string</span></span>        | <span data-ttu-id="9c15a-136">已授予访问权限的 Azure AD 应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="9c15a-136">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="9c15a-137">只读。</span><span class="sxs-lookup"><span data-stu-id="9c15a-137">Read-only.</span></span>   |
| <span data-ttu-id="9c15a-138">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="9c15a-138">resourceAppId</span></span>   | <span data-ttu-id="9c15a-139">string</span><span class="sxs-lookup"><span data-stu-id="9c15a-139">string</span></span>        | <span data-ttu-id="9c15a-140">托管资源的 Azure AD 应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="9c15a-140">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="9c15a-141">只读。</span><span class="sxs-lookup"><span data-stu-id="9c15a-141">Read-only.</span></span>                        |
| <span data-ttu-id="9c15a-142">permissionType</span><span class="sxs-lookup"><span data-stu-id="9c15a-142">permissionType</span></span>  | <span data-ttu-id="9c15a-143">string</span><span class="sxs-lookup"><span data-stu-id="9c15a-143">string</span></span>        | <span data-ttu-id="9c15a-144">权限的类型。</span><span class="sxs-lookup"><span data-stu-id="9c15a-144">The type of permission.</span></span> <span data-ttu-id="9c15a-145">可能的值是：`Application`、`Delegated`。</span><span class="sxs-lookup"><span data-stu-id="9c15a-145">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="9c15a-146">只读。</span><span class="sxs-lookup"><span data-stu-id="9c15a-146">Read-only.</span></span> |
| <span data-ttu-id="9c15a-147">permission</span><span class="sxs-lookup"><span data-stu-id="9c15a-147">permission</span></span>      | <span data-ttu-id="9c15a-148">string</span><span class="sxs-lookup"><span data-stu-id="9c15a-148">string</span></span>        | <span data-ttu-id="9c15a-149">权限的名称。</span><span class="sxs-lookup"><span data-stu-id="9c15a-149">The name of the permission.</span></span> <span data-ttu-id="9c15a-150">只读。</span><span class="sxs-lookup"><span data-stu-id="9c15a-150">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="9c15a-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9c15a-151">JSON representation</span></span>

<span data-ttu-id="9c15a-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9c15a-152">The following is a JSON representation of the resource.</span></span>

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


