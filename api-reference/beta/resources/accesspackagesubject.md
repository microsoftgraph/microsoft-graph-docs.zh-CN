---
title: accessPackageSubject 资源类型
description: 在 Azure AD 权限管理中，访问包分配的主题。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0b37d91ad5669a0a87cef91893babf392f2f309b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939402"
---
# <a name="accesspackagesubject-resource-type"></a><span data-ttu-id="64cea-103">accessPackageSubject 资源类型</span><span class="sxs-lookup"><span data-stu-id="64cea-103">accessPackageSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64cea-104">在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包主题是可以配置为请求或分配访问包的用户、服务主体或其他实体。</span><span class="sxs-lookup"><span data-stu-id="64cea-104">In [Azure AD entitlement management](entitlementmanagement-root.md), an access package subject is a user, service principal, or other entity that can be configured to request or be assigned an access package.</span></span>

## <a name="properties"></a><span data-ttu-id="64cea-105">属性</span><span class="sxs-lookup"><span data-stu-id="64cea-105">Properties</span></span>

| <span data-ttu-id="64cea-106">属性</span><span class="sxs-lookup"><span data-stu-id="64cea-106">Property</span></span>     | <span data-ttu-id="64cea-107">类型</span><span class="sxs-lookup"><span data-stu-id="64cea-107">Type</span></span>        | <span data-ttu-id="64cea-108">说明</span><span class="sxs-lookup"><span data-stu-id="64cea-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="64cea-109">displayName</span><span class="sxs-lookup"><span data-stu-id="64cea-109">displayName</span></span>|<span data-ttu-id="64cea-110">字符串</span><span class="sxs-lookup"><span data-stu-id="64cea-110">String</span></span>|<span data-ttu-id="64cea-111">主题的显示名称。</span><span class="sxs-lookup"><span data-stu-id="64cea-111">The display name of the subject.</span></span>|
|<span data-ttu-id="64cea-112">email</span><span class="sxs-lookup"><span data-stu-id="64cea-112">email</span></span>|<span data-ttu-id="64cea-113">String</span><span class="sxs-lookup"><span data-stu-id="64cea-113">String</span></span>|<span data-ttu-id="64cea-114">主题的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="64cea-114">The email address of the subject.</span></span>|
|<span data-ttu-id="64cea-115">id</span><span class="sxs-lookup"><span data-stu-id="64cea-115">id</span></span>|<span data-ttu-id="64cea-116">字符串</span><span class="sxs-lookup"><span data-stu-id="64cea-116">String</span></span>| <span data-ttu-id="64cea-117">只读。</span><span class="sxs-lookup"><span data-stu-id="64cea-117">Read-only.</span></span>|
|<span data-ttu-id="64cea-118">objectId</span><span class="sxs-lookup"><span data-stu-id="64cea-118">objectId</span></span>|<span data-ttu-id="64cea-119">字符串</span><span class="sxs-lookup"><span data-stu-id="64cea-119">String</span></span>|<span data-ttu-id="64cea-120">主题的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="64cea-120">The object ID of the subject.</span></span>|
|<span data-ttu-id="64cea-121">principalName</span><span class="sxs-lookup"><span data-stu-id="64cea-121">principalName</span></span>|<span data-ttu-id="64cea-122">String</span><span class="sxs-lookup"><span data-stu-id="64cea-122">String</span></span>|<span data-ttu-id="64cea-123">主题的主体名称（如果已知）。</span><span class="sxs-lookup"><span data-stu-id="64cea-123">The principal name, if known, of the subject.</span></span>|
|<span data-ttu-id="64cea-124">type</span><span class="sxs-lookup"><span data-stu-id="64cea-124">type</span></span>|<span data-ttu-id="64cea-125">字符串</span><span class="sxs-lookup"><span data-stu-id="64cea-125">String</span></span>|<span data-ttu-id="64cea-126">主题的资源类型。</span><span class="sxs-lookup"><span data-stu-id="64cea-126">The resource type of the subject.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64cea-127">关系</span><span class="sxs-lookup"><span data-stu-id="64cea-127">Relationships</span></span>

<span data-ttu-id="64cea-128">无。</span><span class="sxs-lookup"><span data-stu-id="64cea-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="64cea-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64cea-129">JSON representation</span></span>

<span data-ttu-id="64cea-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64cea-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "baseType": "",
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
