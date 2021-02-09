---
title: accessPackageSubject 资源类型
description: 在 Azure AD 权利管理中，访问包分配的主题。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3f5bbd3147b27193d8a8e8a3e4bea3914719124c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161780"
---
# <a name="accesspackagesubject-resource-type"></a><span data-ttu-id="9172b-103">accessPackageSubject 资源类型</span><span class="sxs-lookup"><span data-stu-id="9172b-103">accessPackageSubject resource type</span></span>

<span data-ttu-id="9172b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9172b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9172b-105">在 [Azure AD 权利](entitlementmanagement-root.md)管理中，访问包主题是可配置为请求或分配访问包的用户、服务主体或其他实体。</span><span class="sxs-lookup"><span data-stu-id="9172b-105">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package subject is a user, service principal, or other entity that can be configured to request or be assigned an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="9172b-106">属性</span><span class="sxs-lookup"><span data-stu-id="9172b-106">Properties</span></span>

| <span data-ttu-id="9172b-107">属性</span><span class="sxs-lookup"><span data-stu-id="9172b-107">Property</span></span>     | <span data-ttu-id="9172b-108">类型</span><span class="sxs-lookup"><span data-stu-id="9172b-108">Type</span></span>        | <span data-ttu-id="9172b-109">说明</span><span class="sxs-lookup"><span data-stu-id="9172b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9172b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9172b-110">displayName</span></span>|<span data-ttu-id="9172b-111">String</span><span class="sxs-lookup"><span data-stu-id="9172b-111">String</span></span>|<span data-ttu-id="9172b-112">主题显示名称。</span><span class="sxs-lookup"><span data-stu-id="9172b-112">The display name of the subject.</span></span>|
|<span data-ttu-id="9172b-113">email</span><span class="sxs-lookup"><span data-stu-id="9172b-113">email</span></span>|<span data-ttu-id="9172b-114">String</span><span class="sxs-lookup"><span data-stu-id="9172b-114">String</span></span>|<span data-ttu-id="9172b-115">主题的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9172b-115">The email address of the subject.</span></span>|
|<span data-ttu-id="9172b-116">id</span><span class="sxs-lookup"><span data-stu-id="9172b-116">id</span></span>|<span data-ttu-id="9172b-117">String</span><span class="sxs-lookup"><span data-stu-id="9172b-117">String</span></span>| <span data-ttu-id="9172b-118">只读。</span><span class="sxs-lookup"><span data-stu-id="9172b-118">Read-only.</span></span>|
|<span data-ttu-id="9172b-119">objectId</span><span class="sxs-lookup"><span data-stu-id="9172b-119">objectId</span></span>|<span data-ttu-id="9172b-120">String</span><span class="sxs-lookup"><span data-stu-id="9172b-120">String</span></span>|<span data-ttu-id="9172b-121">主题的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="9172b-121">The object ID of the subject.</span></span>|
|<span data-ttu-id="9172b-122">principalName</span><span class="sxs-lookup"><span data-stu-id="9172b-122">principalName</span></span>|<span data-ttu-id="9172b-123">String</span><span class="sxs-lookup"><span data-stu-id="9172b-123">String</span></span>|<span data-ttu-id="9172b-124">主题的主体名称（如果已知）。</span><span class="sxs-lookup"><span data-stu-id="9172b-124">The principal name, if known, of the subject.</span></span>|
|<span data-ttu-id="9172b-125">type</span><span class="sxs-lookup"><span data-stu-id="9172b-125">type</span></span>|<span data-ttu-id="9172b-126">String</span><span class="sxs-lookup"><span data-stu-id="9172b-126">String</span></span>|<span data-ttu-id="9172b-127">主题的资源类型。</span><span class="sxs-lookup"><span data-stu-id="9172b-127">The resource type of the subject.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9172b-128">关系</span><span class="sxs-lookup"><span data-stu-id="9172b-128">Relationships</span></span>

<span data-ttu-id="9172b-129">无。</span><span class="sxs-lookup"><span data-stu-id="9172b-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9172b-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9172b-130">JSON representation</span></span>

<span data-ttu-id="9172b-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9172b-131">The following is a JSON representation of the resource.</span></span>

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


