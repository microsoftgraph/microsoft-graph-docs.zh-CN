---
title: accessPackageSubject 资源类型
description: 在 Azure AD 权利管理中，访问包分配的主题。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0adfca021ec463029a4b35c047ac85f8ce52921b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467055"
---
# <a name="accesspackagesubject-resource-type"></a><span data-ttu-id="19ee9-103">accessPackageSubject 资源类型</span><span class="sxs-lookup"><span data-stu-id="19ee9-103">accessPackageSubject resource type</span></span>

<span data-ttu-id="19ee9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19ee9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19ee9-105">在 [Azure AD 权利](entitlementmanagement-root.md)管理中，访问包主题是可配置为请求或分配访问包的用户、服务主体或其他实体。</span><span class="sxs-lookup"><span data-stu-id="19ee9-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package subject is a user, service principal, or other entity that can be configured to request or be assigned an access package.</span></span>  <span data-ttu-id="19ee9-106">它可以表示来自尚未在租户中的已连接组织的请求者。</span><span class="sxs-lookup"><span data-stu-id="19ee9-106">It may represent a requestor from a connected organization who is not yet in the tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="19ee9-107">属性</span><span class="sxs-lookup"><span data-stu-id="19ee9-107">Properties</span></span>

| <span data-ttu-id="19ee9-108">属性</span><span class="sxs-lookup"><span data-stu-id="19ee9-108">Property</span></span>     | <span data-ttu-id="19ee9-109">类型</span><span class="sxs-lookup"><span data-stu-id="19ee9-109">Type</span></span>        | <span data-ttu-id="19ee9-110">说明</span><span class="sxs-lookup"><span data-stu-id="19ee9-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="19ee9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="19ee9-111">displayName</span></span>|<span data-ttu-id="19ee9-112">String</span><span class="sxs-lookup"><span data-stu-id="19ee9-112">String</span></span>|<span data-ttu-id="19ee9-113">主题显示名称。</span><span class="sxs-lookup"><span data-stu-id="19ee9-113">The display name of the subject.</span></span>|
|<span data-ttu-id="19ee9-114">email</span><span class="sxs-lookup"><span data-stu-id="19ee9-114">email</span></span>|<span data-ttu-id="19ee9-115">String</span><span class="sxs-lookup"><span data-stu-id="19ee9-115">String</span></span>|<span data-ttu-id="19ee9-116">主题的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="19ee9-116">The email address of the subject.</span></span>|
|<span data-ttu-id="19ee9-117">id</span><span class="sxs-lookup"><span data-stu-id="19ee9-117">id</span></span>|<span data-ttu-id="19ee9-118">String</span><span class="sxs-lookup"><span data-stu-id="19ee9-118">String</span></span>| <span data-ttu-id="19ee9-119">只读。</span><span class="sxs-lookup"><span data-stu-id="19ee9-119">Read-only.</span></span>|
|<span data-ttu-id="19ee9-120">objectId</span><span class="sxs-lookup"><span data-stu-id="19ee9-120">objectId</span></span>|<span data-ttu-id="19ee9-121">String</span><span class="sxs-lookup"><span data-stu-id="19ee9-121">String</span></span>|<span data-ttu-id="19ee9-122">主题的对象标识符。</span><span class="sxs-lookup"><span data-stu-id="19ee9-122">The object identifier of the subject.</span></span> <span data-ttu-id="19ee9-123">`null` 如果主题不是租户中的用户。</span><span class="sxs-lookup"><span data-stu-id="19ee9-123">`null` if the subject is not yet a user in the tenant.</span></span>|
|<span data-ttu-id="19ee9-124">principalName</span><span class="sxs-lookup"><span data-stu-id="19ee9-124">principalName</span></span>|<span data-ttu-id="19ee9-125">String</span><span class="sxs-lookup"><span data-stu-id="19ee9-125">String</span></span>|<span data-ttu-id="19ee9-126">主题的主体名称（如果已知）。</span><span class="sxs-lookup"><span data-stu-id="19ee9-126">The principal name, if known, of the subject.</span></span>|
|<span data-ttu-id="19ee9-127">type</span><span class="sxs-lookup"><span data-stu-id="19ee9-127">type</span></span>|<span data-ttu-id="19ee9-128">String</span><span class="sxs-lookup"><span data-stu-id="19ee9-128">String</span></span>|<span data-ttu-id="19ee9-129">主题的资源类型。</span><span class="sxs-lookup"><span data-stu-id="19ee9-129">The resource type of the subject.</span></span>|
|<span data-ttu-id="19ee9-130">connectedOrganizationId</span><span class="sxs-lookup"><span data-stu-id="19ee9-130">connectedOrganizationId</span></span>|<span data-ttu-id="19ee9-131">String</span><span class="sxs-lookup"><span data-stu-id="19ee9-131">String</span></span>|<span data-ttu-id="19ee9-132">主题的已连接组织的标识符。</span><span class="sxs-lookup"><span data-stu-id="19ee9-132">The identifier of the connected organization of the subject.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19ee9-133">关系</span><span class="sxs-lookup"><span data-stu-id="19ee9-133">Relationships</span></span>

| <span data-ttu-id="19ee9-134">关系</span><span class="sxs-lookup"><span data-stu-id="19ee9-134">Relationship</span></span> | <span data-ttu-id="19ee9-135">类型</span><span class="sxs-lookup"><span data-stu-id="19ee9-135">Type</span></span>        | <span data-ttu-id="19ee9-136">说明</span><span class="sxs-lookup"><span data-stu-id="19ee9-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="19ee9-137">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="19ee9-137">connectedOrganization</span></span>|[<span data-ttu-id="19ee9-138">connectedOrganization</span><span class="sxs-lookup"><span data-stu-id="19ee9-138">connectedOrganization</span></span>](connectedorganization.md)| <span data-ttu-id="19ee9-139">主题的已连接组织。</span><span class="sxs-lookup"><span data-stu-id="19ee9-139">The connected organization of the subject.</span></span> <span data-ttu-id="19ee9-140">只读。</span><span class="sxs-lookup"><span data-stu-id="19ee9-140">Read-only.</span></span> <span data-ttu-id="19ee9-141">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="19ee9-141">Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="19ee9-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19ee9-142">JSON representation</span></span>

<span data-ttu-id="19ee9-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19ee9-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "Administrator",
  "email": "admin@contoso.com",
  "id": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
  "objectId": "cc754ed5-f598-45c0-aaf0-fc2f2eb1838f",
  "principalName": "admin@domain.contoso.com",
  "type": "User"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageSubject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

