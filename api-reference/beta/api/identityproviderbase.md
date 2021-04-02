---
title: identityProviderBase 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的身份提供程序。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: namkedia
ms.openlocfilehash: 71c6d58e9ad70773df39adc7d2a91393d64cd460
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491059"
---
# <a name="identityproviderbase-resource-type"></a><span data-ttu-id="eef7b-103">identityProviderBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="eef7b-103">identityProviderBase resource type</span></span>
<span data-ttu-id="eef7b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eef7b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eef7b-105">对 Azure Active Directory 租户和 Azure AD B2C 租户都标识具有[外部标识](/azure/active-directory/external-identities/)的身份提供程序。</span><span class="sxs-lookup"><span data-stu-id="eef7b-105">Represents identity providers with [External Identities](/azure/active-directory/external-identities/) for both Azure Active Directory tenant and an Azure AD B2C tenant.</span></span>

## <a name="methods"></a><span data-ttu-id="eef7b-106">方法</span><span class="sxs-lookup"><span data-stu-id="eef7b-106">Methods</span></span>

| <span data-ttu-id="eef7b-107">方法</span><span class="sxs-lookup"><span data-stu-id="eef7b-107">Method</span></span>       | <span data-ttu-id="eef7b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="eef7b-108">Return Type</span></span>  |<span data-ttu-id="eef7b-109">Description</span><span class="sxs-lookup"><span data-stu-id="eef7b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eef7b-110">List</span><span class="sxs-lookup"><span data-stu-id="eef7b-110">List</span></span>](../api/identityproviderbase-list.md)|<span data-ttu-id="eef7b-111">identityProviderBase 集合</span><span class="sxs-lookup"><span data-stu-id="eef7b-111">identityProviderBase collection</span></span>|<span data-ttu-id="eef7b-112">检索在租户中配置的所有标识提供程序。</span><span class="sxs-lookup"><span data-stu-id="eef7b-112">Retrieve all identity providers configured in a tenant.</span></span>|
|[<span data-ttu-id="eef7b-113">列出可用的提供程序类型</span><span class="sxs-lookup"><span data-stu-id="eef7b-113">List available provider types</span></span>](../api/identityproviderbase-list-availableprovidertypes.md)|<span data-ttu-id="eef7b-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="eef7b-114">String collection</span></span>|<span data-ttu-id="eef7b-115">检索所有可用的身份提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="eef7b-115">Retrieve all available identity provider types.</span></span>|

## <a name="properties"></a><span data-ttu-id="eef7b-116">属性</span><span class="sxs-lookup"><span data-stu-id="eef7b-116">Properties</span></span>

|<span data-ttu-id="eef7b-117">属性</span><span class="sxs-lookup"><span data-stu-id="eef7b-117">Property</span></span>|<span data-ttu-id="eef7b-118">类型</span><span class="sxs-lookup"><span data-stu-id="eef7b-118">Type</span></span>|<span data-ttu-id="eef7b-119">说明</span><span class="sxs-lookup"><span data-stu-id="eef7b-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eef7b-120">id</span><span class="sxs-lookup"><span data-stu-id="eef7b-120">id</span></span>|<span data-ttu-id="eef7b-121">字符串</span><span class="sxs-lookup"><span data-stu-id="eef7b-121">String</span></span>|<span data-ttu-id="eef7b-122">标识提供程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="eef7b-122">The ID of the identity provider.</span></span>|
|<span data-ttu-id="eef7b-123">displayName</span><span class="sxs-lookup"><span data-stu-id="eef7b-123">displayName</span></span>|<span data-ttu-id="eef7b-124">字符串</span><span class="sxs-lookup"><span data-stu-id="eef7b-124">String</span></span>|<span data-ttu-id="eef7b-125">标识提供程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="eef7b-125">The display name of the identity provider.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eef7b-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eef7b-126">JSON representation</span></span>

<span data-ttu-id="eef7b-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eef7b-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityProviderBase"
} -->

```json
{
    "id": "String",
    "displayName": "String"
}
```
