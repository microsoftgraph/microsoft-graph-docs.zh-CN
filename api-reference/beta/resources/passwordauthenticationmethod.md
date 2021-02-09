---
title: passwordAuthenticationMethod 资源类型
description: 向用户注册的密码的表示形式。
localization_priority: Normal
author: mmcla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 92e135b74bc68662749376298b4be44155b577b2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156691"
---
# <a name="passwordauthenticationmethod-resource-type"></a><span data-ttu-id="94a60-103">passwordAuthenticationMethod 资源类型</span><span class="sxs-lookup"><span data-stu-id="94a60-103">passwordAuthenticationMethod resource type</span></span>

<span data-ttu-id="94a60-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94a60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94a60-105">用户密码的表示形式。</span><span class="sxs-lookup"><span data-stu-id="94a60-105">A representation of a user's password.</span></span> <span data-ttu-id="94a60-106">出于安全考虑，从不会在对象中返回密码本身，但可以采取措施重置密码。</span><span class="sxs-lookup"><span data-stu-id="94a60-106">For security, the password itself will never be returned in the object, but action can be taken to reset a password.</span></span>

## <a name="methods"></a><span data-ttu-id="94a60-107">方法</span><span class="sxs-lookup"><span data-stu-id="94a60-107">Methods</span></span>

| <span data-ttu-id="94a60-108">方法</span><span class="sxs-lookup"><span data-stu-id="94a60-108">Method</span></span>       | <span data-ttu-id="94a60-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="94a60-109">Return Type</span></span> | <span data-ttu-id="94a60-110">说明</span><span class="sxs-lookup"><span data-stu-id="94a60-110">Description</span></span> |
|:-------------|:------------|:------------|
|[<span data-ttu-id="94a60-111">列出 passwordAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="94a60-111">List passwordAuthenticationMethods</span></span>](../api/authentication-list-passwordmethods.md) | <span data-ttu-id="94a60-112">[passwordAuthenticationMethod](passwordauthenticationmethod.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94a60-112">[passwordAuthenticationMethod](passwordauthenticationmethod.md) collection</span></span> | <span data-ttu-id="94a60-113">读取该用户的所有 **passwordAuthenticationMethod** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94a60-113">Read the properties and relationships of all of this user's **passwordAuthenticationMethod** objects.</span></span> |
|[<span data-ttu-id="94a60-114">获取 passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="94a60-114">Get passwordAuthenticationMethod</span></span>](../api/passwordauthenticationmethod-get.md) | [<span data-ttu-id="94a60-115">passwordAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="94a60-115">passwordAuthenticationMethod</span></span>](passwordauthenticationmethod.md) | <span data-ttu-id="94a60-116">读取 **passwordAuthenticationMethod 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="94a60-116">Read the properties and relationships of a **passwordAuthenticationMethod** object.</span></span> |
|[<span data-ttu-id="94a60-117">重置密码</span><span class="sxs-lookup"><span data-stu-id="94a60-117">Reset password</span></span>](../api/passwordauthenticationmethod-resetpassword.md)|<span data-ttu-id="94a60-118">无</span><span class="sxs-lookup"><span data-stu-id="94a60-118">None</span></span>|<span data-ttu-id="94a60-119">在云中重置用户密码，如果同步，则重置本地密码。</span><span class="sxs-lookup"><span data-stu-id="94a60-119">Reset a user's password in the cloud and, if synced, on-premises.</span></span>|

## <a name="properties"></a><span data-ttu-id="94a60-120">属性</span><span class="sxs-lookup"><span data-stu-id="94a60-120">Properties</span></span>

| <span data-ttu-id="94a60-121">属性</span><span class="sxs-lookup"><span data-stu-id="94a60-121">Property</span></span>     | <span data-ttu-id="94a60-122">类型</span><span class="sxs-lookup"><span data-stu-id="94a60-122">Type</span></span>        | <span data-ttu-id="94a60-123">说明</span><span class="sxs-lookup"><span data-stu-id="94a60-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="94a60-124">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="94a60-124">creationDateTime</span></span>|<span data-ttu-id="94a60-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94a60-125">DateTimeOffset</span></span>|<span data-ttu-id="94a60-126">上次更新此密码的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="94a60-126">The date and time when this password was last updated.</span></span> <span data-ttu-id="94a60-127">此属性当前未填充。</span><span class="sxs-lookup"><span data-stu-id="94a60-127">This property is currently not populated.</span></span> <span data-ttu-id="94a60-128">只读。</span><span class="sxs-lookup"><span data-stu-id="94a60-128">Read-only.</span></span> <span data-ttu-id="94a60-129">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="94a60-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="94a60-130">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="94a60-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="94a60-131">id</span><span class="sxs-lookup"><span data-stu-id="94a60-131">id</span></span>|<span data-ttu-id="94a60-132">String</span><span class="sxs-lookup"><span data-stu-id="94a60-132">String</span></span>| <span data-ttu-id="94a60-133">向此用户注册的此密码的标识符。</span><span class="sxs-lookup"><span data-stu-id="94a60-133">The identifier of this password registered to this user.</span></span> <span data-ttu-id="94a60-134">只读。</span><span class="sxs-lookup"><span data-stu-id="94a60-134">Read-only.</span></span>|
|<span data-ttu-id="94a60-135">密码</span><span class="sxs-lookup"><span data-stu-id="94a60-135">password</span></span>|<span data-ttu-id="94a60-136">String</span><span class="sxs-lookup"><span data-stu-id="94a60-136">String</span></span>|<span data-ttu-id="94a60-137">为了安全，密码始终从 LIST 或 GET 操作返回为 null。</span><span class="sxs-lookup"><span data-stu-id="94a60-137">For security, the password is always returned as null from a LIST or GET operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94a60-138">关系</span><span class="sxs-lookup"><span data-stu-id="94a60-138">Relationships</span></span>

<span data-ttu-id="94a60-139">无。</span><span class="sxs-lookup"><span data-stu-id="94a60-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="94a60-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94a60-140">JSON representation</span></span>

<span data-ttu-id="94a60-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94a60-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordAuthenticationMethod",
  "keyProperty": "id"
}-->

```json
{
  "creationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "password": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordAuthenticationMethod resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


