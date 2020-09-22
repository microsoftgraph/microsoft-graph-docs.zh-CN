---
title: objectIdentity 资源类型
description: 表示用于登录到用户帐户的标识。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: krbain
ms.openlocfilehash: d2667b8750473ea3e778c078159a1fc9397af1b7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094979"
---
# <a name="objectidentity-resource-type"></a><span data-ttu-id="de596-103">objectIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="de596-103">objectIdentity resource type</span></span>

<span data-ttu-id="de596-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de596-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de596-105">表示用于登录到用户帐户的标识。</span><span class="sxs-lookup"><span data-stu-id="de596-105">Represents an identity used to sign in to a user account.</span></span> <span data-ttu-id="de596-106">标识可由 Microsoft、组织或由与用户帐户关联的社会身份提供商（如 Facebook、Google 或 Microsoft）提供。</span><span class="sxs-lookup"><span data-stu-id="de596-106">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, or Microsoft, that are tied to a user account.</span></span> <span data-ttu-id="de596-107">这样一来，用户就可以使用任何相关标识登录到用户帐户。</span><span class="sxs-lookup"><span data-stu-id="de596-107">This enables the user to sign in to the user account with any of those associated identities.</span></span>

<span data-ttu-id="de596-108">[User](user.md)资源的**标识**属性是一个**objectIdentity**对象。</span><span class="sxs-lookup"><span data-stu-id="de596-108">The **identities** property of the [user](user.md) resource is an **objectIdentity** object.</span></span>

## <a name="properties"></a><span data-ttu-id="de596-109">属性</span><span class="sxs-lookup"><span data-stu-id="de596-109">Properties</span></span>

| <span data-ttu-id="de596-110">属性</span><span class="sxs-lookup"><span data-stu-id="de596-110">Property</span></span>   | <span data-ttu-id="de596-111">类型</span><span class="sxs-lookup"><span data-stu-id="de596-111">Type</span></span> |<span data-ttu-id="de596-112">说明</span><span class="sxs-lookup"><span data-stu-id="de596-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de596-113">signInType</span><span class="sxs-lookup"><span data-stu-id="de596-113">signInType</span></span>|<span data-ttu-id="de596-114">string</span><span class="sxs-lookup"><span data-stu-id="de596-114">string</span></span>| <span data-ttu-id="de596-115">指定目录中的用户登录类型，如 `emailAddress` `userName` 或 `federated` 。</span><span class="sxs-lookup"><span data-stu-id="de596-115">Specifies the user sign-in types in your directory, such as `emailAddress`, `userName` or `federated`.</span></span> <span data-ttu-id="de596-116">此处， `federated` 表示颁发者的用户的唯一标识符，该标识符可以采用颁发者选择的任何格式。</span><span class="sxs-lookup"><span data-stu-id="de596-116">Here, `federated` represents a unique identifier for a user from an issuer, that can be in any format chosen by the issuer.</span></span> <span data-ttu-id="de596-117">当登录类型设置为或时，对 **issuerAssignedId** 强制执行其他验证 `emailAddress` `userName` 。</span><span class="sxs-lookup"><span data-stu-id="de596-117">Additional validation is enforced on **issuerAssignedId** when the sign-in type is set to `emailAddress` or `userName`.</span></span> <span data-ttu-id="de596-118">此属性还可以设置为任何自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="de596-118">This property can also be set to any custom string.</span></span>|
|<span data-ttu-id="de596-119">常用</span><span class="sxs-lookup"><span data-stu-id="de596-119">issuer</span></span>|<span data-ttu-id="de596-120">string</span><span class="sxs-lookup"><span data-stu-id="de596-120">string</span></span>|<span data-ttu-id="de596-121">指定标识的颁发者，例如 `facebook.com` 。</span><span class="sxs-lookup"><span data-stu-id="de596-121">Specifies the issuer of the identity, for example `facebook.com`.</span></span><br><span data-ttu-id="de596-122">对于不) **signInType** 的本地帐户 (`federated` ，此属性是本地 B2C 租户默认域名（例如） `contoso.onmicrosoft.com` 。</span><span class="sxs-lookup"><span data-stu-id="de596-122">For local accounts (where **signInType** is not `federated`), this property is the local B2C tenant default domain name, for example `contoso.onmicrosoft.com`.</span></span><br><span data-ttu-id="de596-123">对于来自其他 Azure AD 组织的外部用户，这将是联合组织的域，例如 `contoso.com` 。</span><span class="sxs-lookup"><span data-stu-id="de596-123">For external users from other Azure AD organization, this will be the domain of the federated organization, for example `contoso.com`.</span></span><br><br><span data-ttu-id="de596-124">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="de596-124">Supports `$filter`.</span></span> <span data-ttu-id="de596-125">512字符限制。</span><span class="sxs-lookup"><span data-stu-id="de596-125">512 character limit.</span></span>|
|<span data-ttu-id="de596-126">issuerAssignedId</span><span class="sxs-lookup"><span data-stu-id="de596-126">issuerAssignedId</span></span>|<span data-ttu-id="de596-127">string</span><span class="sxs-lookup"><span data-stu-id="de596-127">string</span></span>|<span data-ttu-id="de596-128">指定由颁发者分配给用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="de596-128">Specifies the unique identifier assigned to the user by the issuer.</span></span> <span data-ttu-id="de596-129">**颁发者**和**issuerAssignedId**的组合在组织中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="de596-129">The combination of **issuer** and **issuerAssignedId** must be unique within the organization.</span></span> <span data-ttu-id="de596-130">表示用户的登录名，当 **signInType** 设置为 `emailAddress` 或 `userName` (也称为 "本地帐户) " 时。</span><span class="sxs-lookup"><span data-stu-id="de596-130">Represents the sign-in name for the user, when **signInType** is set to `emailAddress` or `userName` (also known as local accounts).</span></span><br><span data-ttu-id="de596-131">当 **signInType** 设置为时：</span><span class="sxs-lookup"><span data-stu-id="de596-131">When **signInType** is set to:</span></span> <ul><li><span data-ttu-id="de596-132">`emailAddress`， (或以 `emailAddress` like) 开头。 `emailAddress1` **issuerAssignedId** 必须是有效的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="de596-132">`emailAddress`, (or starts with `emailAddress` like `emailAddress1`) **issuerAssignedId** must be a valid email address</span></span></li><li><span data-ttu-id="de596-133">`userName`， **issuerAssignedId** 必须是 [电子邮件地址的有效本地部分](https://tools.ietf.org/html/rfc3696#section-3)</span><span class="sxs-lookup"><span data-stu-id="de596-133">`userName`, **issuerAssignedId** must be a valid [local part of an email address](https://tools.ietf.org/html/rfc3696#section-3)</span></span></li></ul><span data-ttu-id="de596-134">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="de596-134">Supports `$filter`.</span></span> <span data-ttu-id="de596-135">512字符限制。</span><span class="sxs-lookup"><span data-stu-id="de596-135">512 character limit.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de596-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de596-136">JSON representation</span></span>

<span data-ttu-id="de596-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de596-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.objectIdentity"
}-->

```json
{
  "signInType": "string",
  "issuer": "string",
  "issuerAssignedId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "objectIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


