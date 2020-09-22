---
title: passwordSingleSignOnField 资源类型
description: 用于捕获密码 SSO 凭据的字段
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d79f2347acabae0323e008a43adb7938d70d3768
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998192"
---
# <a name="passwordsinglesignonfield-resource-type"></a><span data-ttu-id="678ec-103">passwordSingleSignOnField 资源类型</span><span class="sxs-lookup"><span data-stu-id="678ec-103">passwordSingleSignOnField resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="678ec-104">包含要捕获以填充基于密码的单一登录的使用凭据的字段。</span><span class="sxs-lookup"><span data-stu-id="678ec-104">Contains the fields to capture to fill the use credentials for Password-based single sign-on.</span></span>

## <a name="properties"></a><span data-ttu-id="678ec-105">属性</span><span class="sxs-lookup"><span data-stu-id="678ec-105">Properties</span></span>

| <span data-ttu-id="678ec-106">属性</span><span class="sxs-lookup"><span data-stu-id="678ec-106">Property</span></span>     | <span data-ttu-id="678ec-107">类型</span><span class="sxs-lookup"><span data-stu-id="678ec-107">Type</span></span>        | <span data-ttu-id="678ec-108">说明</span><span class="sxs-lookup"><span data-stu-id="678ec-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="678ec-109">customizedLabel</span><span class="sxs-lookup"><span data-stu-id="678ec-109">customizedLabel</span></span>|<span data-ttu-id="678ec-110">String</span><span class="sxs-lookup"><span data-stu-id="678ec-110">String</span></span>|<span data-ttu-id="678ec-111">用于自定义的标题/标签覆盖。</span><span class="sxs-lookup"><span data-stu-id="678ec-111">Title/label override for customization.</span></span>|
|<span data-ttu-id="678ec-112">defaultLabel</span><span class="sxs-lookup"><span data-stu-id="678ec-112">defaultLabel</span></span>|<span data-ttu-id="678ec-113">String</span><span class="sxs-lookup"><span data-stu-id="678ec-113">String</span></span>|<span data-ttu-id="678ec-114">未提供 customizedLabel 时将使用的标签。</span><span class="sxs-lookup"><span data-stu-id="678ec-114">Label that would be used if no customizedLabel is provided.</span></span> <span data-ttu-id="678ec-115">只读。</span><span class="sxs-lookup"><span data-stu-id="678ec-115">Read only.</span></span>|
|<span data-ttu-id="678ec-116">fieldId</span><span class="sxs-lookup"><span data-stu-id="678ec-116">fieldId</span></span>|<span data-ttu-id="678ec-117">String</span><span class="sxs-lookup"><span data-stu-id="678ec-117">String</span></span>|<span data-ttu-id="678ec-118">用于标识字段类型的 Id。</span><span class="sxs-lookup"><span data-stu-id="678ec-118">Id used to identity the field type.</span></span> <span data-ttu-id="678ec-119">这是一个内部 id，可能的值为、、、 `param_1` `param_2` `param_userName` `param_password` 。</span><span class="sxs-lookup"><span data-stu-id="678ec-119">This is an internal id and possible values are `param_1`, `param_2`, `param_userName`, `param_password`.</span></span>|
|<span data-ttu-id="678ec-120">type</span><span class="sxs-lookup"><span data-stu-id="678ec-120">type</span></span>|<span data-ttu-id="678ec-121">String</span><span class="sxs-lookup"><span data-stu-id="678ec-121">String</span></span>|   <span data-ttu-id="678ec-122">凭据的类型。</span><span class="sxs-lookup"><span data-stu-id="678ec-122">Type of the credential.</span></span> <span data-ttu-id="678ec-123">值可以是 `text` ， `password` 。</span><span class="sxs-lookup"><span data-stu-id="678ec-123">The values can be `text`, `password`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="678ec-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="678ec-124">JSON representation</span></span>

<span data-ttu-id="678ec-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="678ec-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordSingleSignOnField",
  "baseType": null
}-->

```json
{
  "customizedLabel": "String",
  "defaultLabel": "String",
  "fieldId": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordSingleSignOnField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

