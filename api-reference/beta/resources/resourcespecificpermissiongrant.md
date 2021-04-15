---
title: resourceSpecificPermissionGrant 资源类型
description: 指定特定 Azure AD 应用具有的权限。
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7119d25f25b0e4f382a077ca6a1264dc22e11d5b
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765900"
---
# <a name="resourcespecificpermissiongrant-resource-type"></a><span data-ttu-id="c295a-103">resourceSpecificPermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="c295a-103">resourceSpecificPermissionGrant resource type</span></span>

<span data-ttu-id="c295a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c295a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c295a-105">resourceSpecificPermissionGrant 声明已授予特定 AzureAD 应用的权限，该权限适用于 Microsoft Graph 中的资源实例。</span><span class="sxs-lookup"><span data-stu-id="c295a-105">A resourceSpecificPermissionGrant declares the permission that has been granted to a specific AzureAD app for an instance of a resource in Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="c295a-106">方法</span><span class="sxs-lookup"><span data-stu-id="c295a-106">Methods</span></span>

|  <span data-ttu-id="c295a-107">方法</span><span class="sxs-lookup"><span data-stu-id="c295a-107">Method</span></span>                                                                   |  <span data-ttu-id="c295a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c295a-108">Return Type</span></span>                                                                     | <span data-ttu-id="c295a-109">说明</span><span class="sxs-lookup"><span data-stu-id="c295a-109">Description</span></span>                                                  | 
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------- | :----------------------------------------------------------- |
|[<span data-ttu-id="c295a-110">聊天的列表权限授予</span><span class="sxs-lookup"><span data-stu-id="c295a-110">List permission grants of a chat</span></span>](../api/chat-list-permissiongrants.md)   | <span data-ttu-id="c295a-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c295a-111">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="c295a-112">列出特定聊天中已授予的权限。</span><span class="sxs-lookup"><span data-stu-id="c295a-112">List permissions that have been granted in a specific chat.</span></span>  |
|[<span data-ttu-id="c295a-113">列出组的权限授予</span><span class="sxs-lookup"><span data-stu-id="c295a-113">List permission grants of a group</span></span>](../api/group-list-permissiongrants.md) | <span data-ttu-id="c295a-114">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c295a-114">[resourceSpecificPermissionGrant](resourcespecificpermissiongrant.md) collection</span></span> | <span data-ttu-id="c295a-115">列出特定组中已授予的权限。</span><span class="sxs-lookup"><span data-stu-id="c295a-115">List permissions that have been granted in a specific group.</span></span> |

## <a name="properties"></a><span data-ttu-id="c295a-116">属性</span><span class="sxs-lookup"><span data-stu-id="c295a-116">Properties</span></span>

| <span data-ttu-id="c295a-117">属性</span><span class="sxs-lookup"><span data-stu-id="c295a-117">Property</span></span>        | <span data-ttu-id="c295a-118">类型</span><span class="sxs-lookup"><span data-stu-id="c295a-118">Type</span></span>          | <span data-ttu-id="c295a-119">说明</span><span class="sxs-lookup"><span data-stu-id="c295a-119">Description</span></span>                                                                           |
| :-------------- | :------------ | :------------------------------------------------------------------------------------ |
| <span data-ttu-id="c295a-120">id</span><span class="sxs-lookup"><span data-stu-id="c295a-120">id</span></span>              | <span data-ttu-id="c295a-121">string</span><span class="sxs-lookup"><span data-stu-id="c295a-121">string</span></span>        | <span data-ttu-id="c295a-122">特定于资源的权限授予的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c295a-122">The unique identifier of the resource-specific permission grant.</span></span> <span data-ttu-id="c295a-123">只读。</span><span class="sxs-lookup"><span data-stu-id="c295a-123">Read-only.</span></span>           |
| <span data-ttu-id="c295a-124">deletedDateTime</span><span class="sxs-lookup"><span data-stu-id="c295a-124">deletedDateTime</span></span> | <span data-ttu-id="c295a-125">dateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c295a-125">dateTimeOffset</span></span>| <span data-ttu-id="c295a-126">未使用。</span><span class="sxs-lookup"><span data-stu-id="c295a-126">Not used.</span></span>                                                                             |
| <span data-ttu-id="c295a-127">clientId</span><span class="sxs-lookup"><span data-stu-id="c295a-127">clientId</span></span>        | <span data-ttu-id="c295a-128">字符串</span><span class="sxs-lookup"><span data-stu-id="c295a-128">string</span></span>        | <span data-ttu-id="c295a-129">已授予访问权限的 Azure AD 应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="c295a-129">ID of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="c295a-130">只读。</span><span class="sxs-lookup"><span data-stu-id="c295a-130">Read-only.</span></span>                            |
| <span data-ttu-id="c295a-131">clientAppId</span><span class="sxs-lookup"><span data-stu-id="c295a-131">clientAppId</span></span>     | <span data-ttu-id="c295a-132">字符串</span><span class="sxs-lookup"><span data-stu-id="c295a-132">string</span></span>        | <span data-ttu-id="c295a-133">已授予访问权限的 Azure AD 应用的服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="c295a-133">ID of the service principal of the Azure AD app that has been granted access.</span></span> <span data-ttu-id="c295a-134">只读。</span><span class="sxs-lookup"><span data-stu-id="c295a-134">Read-only.</span></span>   |
| <span data-ttu-id="c295a-135">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="c295a-135">resourceAppId</span></span>   | <span data-ttu-id="c295a-136">字符串</span><span class="sxs-lookup"><span data-stu-id="c295a-136">string</span></span>        | <span data-ttu-id="c295a-137">托管资源的 Azure AD 应用的 ID。</span><span class="sxs-lookup"><span data-stu-id="c295a-137">ID of the Azure AD app that is hosting the resource.</span></span> <span data-ttu-id="c295a-138">只读。</span><span class="sxs-lookup"><span data-stu-id="c295a-138">Read-only.</span></span>                        |
| <span data-ttu-id="c295a-139">permissionType</span><span class="sxs-lookup"><span data-stu-id="c295a-139">permissionType</span></span>  | <span data-ttu-id="c295a-140">字符串</span><span class="sxs-lookup"><span data-stu-id="c295a-140">string</span></span>        | <span data-ttu-id="c295a-141">权限的类型。</span><span class="sxs-lookup"><span data-stu-id="c295a-141">The type of permission.</span></span> <span data-ttu-id="c295a-142">可能的值是：`Application`、`Delegated`。</span><span class="sxs-lookup"><span data-stu-id="c295a-142">Possible values are: `Application`, `Delegated`.</span></span> <span data-ttu-id="c295a-143">只读。</span><span class="sxs-lookup"><span data-stu-id="c295a-143">Read-only.</span></span> |
| <span data-ttu-id="c295a-144">permission</span><span class="sxs-lookup"><span data-stu-id="c295a-144">permission</span></span>      | <span data-ttu-id="c295a-145">字符串</span><span class="sxs-lookup"><span data-stu-id="c295a-145">string</span></span>        | <span data-ttu-id="c295a-146">权限的名称。</span><span class="sxs-lookup"><span data-stu-id="c295a-146">The name of the permission.</span></span> <span data-ttu-id="c295a-147">只读。</span><span class="sxs-lookup"><span data-stu-id="c295a-147">Read-only.</span></span>                                                |

## <a name="json-representation"></a><span data-ttu-id="c295a-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c295a-148">JSON representation</span></span>

<span data-ttu-id="c295a-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c295a-149">The following is a JSON representation of the resource.</span></span>

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


