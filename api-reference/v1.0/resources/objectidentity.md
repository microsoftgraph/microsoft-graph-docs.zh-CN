---
title: objectIdentity 资源类型
description: 表示用于登录用户帐户的标识。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: jpettere
ms.openlocfilehash: 5f989325706ce45fe384370584b645959c153158
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080671"
---
# <a name="objectidentity-resource-type"></a><span data-ttu-id="b467d-103">objectIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="b467d-103">objectIdentity resource type</span></span>

<span data-ttu-id="b467d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b467d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b467d-105">表示用于登录用户帐户的标识。</span><span class="sxs-lookup"><span data-stu-id="b467d-105">Represents an identity used to sign in to a user account.</span></span> <span data-ttu-id="b467d-106">标识由 Microsoft、组织或与用户帐户绑定的社会标识提供者（如 Facebook、Google 或 Microsoft）提供。</span><span class="sxs-lookup"><span data-stu-id="b467d-106">An identity can be provided by Microsoft, by organizations, or by social identity providers such as Facebook, Google, or Microsoft, that are tied to a user account.</span></span> <span data-ttu-id="b467d-107">这使用户能够使用这些关联标识中的任一标识登录用户帐户。</span><span class="sxs-lookup"><span data-stu-id="b467d-107">This enables the user to sign in to the user account with any of those associated identities.</span></span>

<span data-ttu-id="b467d-108">用户 **资源的 identities** [属性是](user.md) **objectIdentity** 对象。</span><span class="sxs-lookup"><span data-stu-id="b467d-108">The **identities** property of the [user](user.md) resource is an **objectIdentity** object.</span></span>

## <a name="properties"></a><span data-ttu-id="b467d-109">属性</span><span class="sxs-lookup"><span data-stu-id="b467d-109">Properties</span></span>

| <span data-ttu-id="b467d-110">属性</span><span class="sxs-lookup"><span data-stu-id="b467d-110">Property</span></span>   | <span data-ttu-id="b467d-111">类型</span><span class="sxs-lookup"><span data-stu-id="b467d-111">Type</span></span> |<span data-ttu-id="b467d-112">说明</span><span class="sxs-lookup"><span data-stu-id="b467d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b467d-113">signInType</span><span class="sxs-lookup"><span data-stu-id="b467d-113">signInType</span></span>|<span data-ttu-id="b467d-114">string</span><span class="sxs-lookup"><span data-stu-id="b467d-114">string</span></span>| <span data-ttu-id="b467d-115">指定目录中的用户登录类型，如 `emailAddress` 或 `userName` `federated` 。</span><span class="sxs-lookup"><span data-stu-id="b467d-115">Specifies the user sign-in types in your directory, such as `emailAddress`, `userName` or `federated`.</span></span> <span data-ttu-id="b467d-116">在此处，表示颁发者中用户的唯一标识符，该标识符可以是颁发者 `federated` 选择的任何格式。</span><span class="sxs-lookup"><span data-stu-id="b467d-116">Here, `federated` represents a unique identifier for a user from an issuer, that can be in any format chosen by the issuer.</span></span> <span data-ttu-id="b467d-117">当登录类型设置为 或 时， **对 issuerAssignedId** 强制执行其他 `emailAddress` 验证 `userName` 。</span><span class="sxs-lookup"><span data-stu-id="b467d-117">Additional validation is enforced on **issuerAssignedId** when the sign-in type is set to `emailAddress` or `userName`.</span></span> <span data-ttu-id="b467d-118">此属性还可以设置为任何自定义字符串。</span><span class="sxs-lookup"><span data-stu-id="b467d-118">This property can also be set to any custom string.</span></span>|
|<span data-ttu-id="b467d-119">issuer</span><span class="sxs-lookup"><span data-stu-id="b467d-119">issuer</span></span>|<span data-ttu-id="b467d-120">string</span><span class="sxs-lookup"><span data-stu-id="b467d-120">string</span></span>|<span data-ttu-id="b467d-121">指定标识的颁发者，例如 `facebook.com` 。</span><span class="sxs-lookup"><span data-stu-id="b467d-121">Specifies the issuer of the identity, for example `facebook.com`.</span></span><br><span data-ttu-id="b467d-122">对于未 (**signInType** 的本地帐户) ，此属性是本地 `federated` B2C 租户的默认域名，例如 `contoso.onmicrosoft.com` 。</span><span class="sxs-lookup"><span data-stu-id="b467d-122">For local accounts (where **signInType** is not `federated`), this property is the local B2C tenant default domain name, for example `contoso.onmicrosoft.com`.</span></span><br><span data-ttu-id="b467d-123">对于来自其他 Azure AD 组织的外部用户，这将是联盟组织的域，例如 `contoso.com` 。</span><span class="sxs-lookup"><span data-stu-id="b467d-123">For external users from other Azure AD organization, this will be the domain of the federated organization, for example `contoso.com`.</span></span><br><br><span data-ttu-id="b467d-124">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="b467d-124">Supports `$filter`.</span></span> <span data-ttu-id="b467d-125">512 个字符限制。</span><span class="sxs-lookup"><span data-stu-id="b467d-125">512 character limit.</span></span>|
|<span data-ttu-id="b467d-126">issuerAssignedId</span><span class="sxs-lookup"><span data-stu-id="b467d-126">issuerAssignedId</span></span>|<span data-ttu-id="b467d-127">string</span><span class="sxs-lookup"><span data-stu-id="b467d-127">string</span></span>|<span data-ttu-id="b467d-128">指定颁发者分配给用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b467d-128">Specifies the unique identifier assigned to the user by the issuer.</span></span> <span data-ttu-id="b467d-129">颁发者 **与** **issuerAssignedId** 的组合在组织中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="b467d-129">The combination of **issuer** and **issuerAssignedId** must be unique within the organization.</span></span> <span data-ttu-id="b467d-130">表示用户的登录名，当 **signInType** 设置为 或 (也称为本地帐户 `emailAddress` `userName`) 。</span><span class="sxs-lookup"><span data-stu-id="b467d-130">Represents the sign-in name for the user, when **signInType** is set to `emailAddress` or `userName` (also known as local accounts).</span></span><br><span data-ttu-id="b467d-131">当 **signInType** 设置为：</span><span class="sxs-lookup"><span data-stu-id="b467d-131">When **signInType** is set to:</span></span> <ul><li><span data-ttu-id="b467d-132">`emailAddress`、 (或以 （如 `emailAddress` `emailAddress1`) **issuerAssignedId）** 开头的自定义字符串必须是有效的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="b467d-132">`emailAddress`, (or a custom string that starts with `emailAddress` like `emailAddress1`) **issuerAssignedId** must be a valid email address</span></span></li><li><span data-ttu-id="b467d-133">`userName`**，issuerAssignedId** 必须是电子邮件地址 [的有效本地部分](https://tools.ietf.org/html/rfc3696#section-3)</span><span class="sxs-lookup"><span data-stu-id="b467d-133">`userName`, **issuerAssignedId** must be a valid [local part of an email address](https://tools.ietf.org/html/rfc3696#section-3)</span></span></li></ul><span data-ttu-id="b467d-134">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="b467d-134">Supports `$filter`.</span></span> <span data-ttu-id="b467d-135">100 个字符限制。</span><span class="sxs-lookup"><span data-stu-id="b467d-135">100 character limit.</span></span>|

><span data-ttu-id="b467d-136">**注意：** 筛选 **identities** 属性时，您必须同时提供 **issuer** 和 **issuerAssignedId**。</span><span class="sxs-lookup"><span data-stu-id="b467d-136">**Note:** When filtering on the **identities** property, you must supply both **issuer** and **issuerAssignedId**.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b467d-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b467d-137">JSON representation</span></span>

<span data-ttu-id="b467d-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b467d-138">The following is a JSON representation of the resource.</span></span>

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

