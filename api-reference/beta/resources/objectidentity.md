---
title: objectIdentity 资源类型
description: 表示用于登录到用户帐户的标识。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c29d7ca1b2b4f20f53ed4be45807eb666002163c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658798"
---
# <a name="objectidentity-resource-type"></a><span data-ttu-id="8e123-103">objectIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e123-103">objectIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8e123-104">表示用于登录到用户帐户的标识。</span><span class="sxs-lookup"><span data-stu-id="8e123-104">Represents an identity used to sign in to a user account.</span></span> <span data-ttu-id="8e123-105">标识可由 Microsoft、组织或由与用户帐户关联的社会身份提供商（如 Facebook、Google 或 Microsoft）提供。</span><span class="sxs-lookup"><span data-stu-id="8e123-105">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, or Microsoft, that are tied to a user account.</span></span> <span data-ttu-id="8e123-106">这样一来，用户就可以使用任何相关标识登录到用户帐户。</span><span class="sxs-lookup"><span data-stu-id="8e123-106">This enables the user to sign in to the user account with any of those associated identities.</span></span>

<span data-ttu-id="8e123-107">[User](user.md)资源的**标识**属性是一个**objectIdentity**对象。</span><span class="sxs-lookup"><span data-stu-id="8e123-107">The **identities** property of the [user](user.md) resource is an **objectIdentity** object.</span></span>

## <a name="properties"></a><span data-ttu-id="8e123-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e123-108">Properties</span></span>

| <span data-ttu-id="8e123-109">属性</span><span class="sxs-lookup"><span data-stu-id="8e123-109">Property</span></span>   | <span data-ttu-id="8e123-110">类型</span><span class="sxs-lookup"><span data-stu-id="8e123-110">Type</span></span> |<span data-ttu-id="8e123-111">说明</span><span class="sxs-lookup"><span data-stu-id="8e123-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8e123-112">signInType</span><span class="sxs-lookup"><span data-stu-id="8e123-112">signInType</span></span>|<span data-ttu-id="8e123-113">string</span><span class="sxs-lookup"><span data-stu-id="8e123-113">string</span></span>| <span data-ttu-id="8e123-114">指定目录中的用户登录类型，如`emailAddress` `userName`或。 `federated`</span><span class="sxs-lookup"><span data-stu-id="8e123-114">Specifies the user sign-in types in your directory, such as `emailAddress`, `userName` or `federated`.</span></span> <span data-ttu-id="8e123-115">此处， `federated`表示颁发者的用户的唯一标识符，该标识符可以采用颁发者选择的任何格式。</span><span class="sxs-lookup"><span data-stu-id="8e123-115">Here, `federated` represents a unique identifier for a user from an issuer, that can be in any format chosen by the issuer.</span></span> <span data-ttu-id="8e123-116">当登录类型设置为\*\*\*\* `emailAddress`或`userName`时，对 issuerAssignedId 强制执行其他验证。</span><span class="sxs-lookup"><span data-stu-id="8e123-116">Additional validation is enforced on **issuerAssignedId** when the sign-in type is set to `emailAddress` or `userName`.</span></span> <span data-ttu-id="8e123-117">此属性还可以设置为任何自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="8e123-117">This property can also be set to any custom string.</span></span>|
|<span data-ttu-id="8e123-118">常用</span><span class="sxs-lookup"><span data-stu-id="8e123-118">issuer</span></span>|<span data-ttu-id="8e123-119">string</span><span class="sxs-lookup"><span data-stu-id="8e123-119">string</span></span>|<span data-ttu-id="8e123-120">指定标识的颁发者，例如`facebook.com`。</span><span class="sxs-lookup"><span data-stu-id="8e123-120">Specifies the issuer of the identity, for example `facebook.com`.</span></span><br><span data-ttu-id="8e123-121">对于本地帐户（其中**signInType**不`federated`是），此属性是本地 B2C 租户默认域名（例如`contoso.onmicrosoft.com`）。</span><span class="sxs-lookup"><span data-stu-id="8e123-121">For local accounts (where **signInType** is not `federated`), this property is the local B2C tenant default domain name, for example `contoso.onmicrosoft.com`.</span></span><br><span data-ttu-id="8e123-122">对于来自其他 Azure AD 组织的外部用户，这将是联合组织的域，例如`contoso.com`。</span><span class="sxs-lookup"><span data-stu-id="8e123-122">For external users from other Azure AD organization, this will be the domain of the federated organization, for example `contoso.com`.</span></span><br><br><span data-ttu-id="8e123-123">支持`$filter`。</span><span class="sxs-lookup"><span data-stu-id="8e123-123">Supports `$filter`.</span></span> <span data-ttu-id="8e123-124">512字符限制。</span><span class="sxs-lookup"><span data-stu-id="8e123-124">512 character limit.</span></span>|
|<span data-ttu-id="8e123-125">issuerAssignedId</span><span class="sxs-lookup"><span data-stu-id="8e123-125">issuerAssignedId</span></span>|<span data-ttu-id="8e123-126">string</span><span class="sxs-lookup"><span data-stu-id="8e123-126">string</span></span>|<span data-ttu-id="8e123-127">指定由颁发者分配给用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8e123-127">Specifies the unique identifier assigned to the user by the issuer.</span></span> <span data-ttu-id="8e123-128">**颁发者**和**issuerAssignedId**的组合在组织中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="8e123-128">The combination of **issuer** and **issuerAssignedId** must be unique within the organization.</span></span> <span data-ttu-id="8e123-129">表示用户的登录名，如果将**signInType**设置为`emailAddress`或`userName` （也称为 "本地帐户"）。</span><span class="sxs-lookup"><span data-stu-id="8e123-129">Represents the sign-in name for the user, when **signInType** is set to `emailAddress` or `userName` (also known as local accounts).</span></span><br><span data-ttu-id="8e123-130">当**signInType**设置为时：</span><span class="sxs-lookup"><span data-stu-id="8e123-130">When **signInType** is set to:</span></span> <ul><li><span data-ttu-id="8e123-131">`emailAddress`（或以`emailAddress` like `emailAddress1`开头） **issuerAssignedId**必须是有效的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="8e123-131">`emailAddress`, (or starts with `emailAddress` like `emailAddress1`) **issuerAssignedId** must be a valid email address</span></span></li><li><span data-ttu-id="8e123-132">`userName`， **issuerAssignedId**必须是[电子邮件地址的有效本地部分](https://tools.ietf.org/html/rfc3696#section-3)</span><span class="sxs-lookup"><span data-stu-id="8e123-132">`userName`, **issuerAssignedId** must be a valid [local part of an email address](https://tools.ietf.org/html/rfc3696#section-3)</span></span></li></ul><span data-ttu-id="8e123-133">支持`$filter`。</span><span class="sxs-lookup"><span data-stu-id="8e123-133">Supports `$filter`.</span></span> <span data-ttu-id="8e123-134">512字符限制。</span><span class="sxs-lookup"><span data-stu-id="8e123-134">512 character limit.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8e123-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e123-135">JSON representation</span></span>

<span data-ttu-id="8e123-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e123-136">The following is a JSON representation of the resource.</span></span>

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
