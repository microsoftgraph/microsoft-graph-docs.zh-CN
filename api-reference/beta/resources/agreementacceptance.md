---
title: agreementAcceptance 资源类型
description: 表示在受 Azure Active Directory （Azure AD）支持的公司自定义使用条款的范围内的用户的当前状态。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 28f3c0adccb853ac8daddca9aaad70a2c0b35e2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508378"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="7c3a0-103">agreementAcceptance 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c3a0-103">agreementAcceptance resource type</span></span>

<span data-ttu-id="7c3a0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7c3a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c3a0-105">表示在受 Azure Active Directory （Azure AD）支持的公司自定义使用条款的范围内的用户的当前状态。</span><span class="sxs-lookup"><span data-stu-id="7c3a0-105">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="7c3a0-106">属性</span><span class="sxs-lookup"><span data-stu-id="7c3a0-106">Properties</span></span>
| <span data-ttu-id="7c3a0-107">属性</span><span class="sxs-lookup"><span data-stu-id="7c3a0-107">Property</span></span>     | <span data-ttu-id="7c3a0-108">类型</span><span class="sxs-lookup"><span data-stu-id="7c3a0-108">Type</span></span>        | <span data-ttu-id="7c3a0-109">说明</span><span class="sxs-lookup"><span data-stu-id="7c3a0-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7c3a0-110">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="7c3a0-110">agreementFileId</span></span>|<span data-ttu-id="7c3a0-111">String</span><span class="sxs-lookup"><span data-stu-id="7c3a0-111">String</span></span>|<span data-ttu-id="7c3a0-112">用户接受的协议文件的 ID。</span><span class="sxs-lookup"><span data-stu-id="7c3a0-112">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="7c3a0-113">agreementId</span><span class="sxs-lookup"><span data-stu-id="7c3a0-113">agreementId</span></span>|<span data-ttu-id="7c3a0-114">String</span><span class="sxs-lookup"><span data-stu-id="7c3a0-114">String</span></span>|<span data-ttu-id="7c3a0-115">协议的 ID。</span><span class="sxs-lookup"><span data-stu-id="7c3a0-115">ID of the agreement.</span></span>|
|<span data-ttu-id="7c3a0-116">id</span><span class="sxs-lookup"><span data-stu-id="7c3a0-116">id</span></span>|<span data-ttu-id="7c3a0-117">String</span><span class="sxs-lookup"><span data-stu-id="7c3a0-117">String</span></span>| <span data-ttu-id="7c3a0-118">只读。</span><span class="sxs-lookup"><span data-stu-id="7c3a0-118">Read-only.</span></span>|
|<span data-ttu-id="7c3a0-119">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="7c3a0-119">recordedDateTime</span></span>|<span data-ttu-id="7c3a0-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7c3a0-120">DateTimeOffset</span></span>|<span data-ttu-id="7c3a0-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7c3a0-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7c3a0-123">state</span><span class="sxs-lookup"><span data-stu-id="7c3a0-123">state</span></span>|<span data-ttu-id="7c3a0-124">string</span><span class="sxs-lookup"><span data-stu-id="7c3a0-124">string</span></span>| <span data-ttu-id="7c3a0-125">可取值为：`accepted`、`declined`。</span><span class="sxs-lookup"><span data-stu-id="7c3a0-125">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="7c3a0-126">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7c3a0-126">userDisplayName</span></span>|<span data-ttu-id="7c3a0-127">String</span><span class="sxs-lookup"><span data-stu-id="7c3a0-127">String</span></span>|<span data-ttu-id="7c3a0-128">记录接受时的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="7c3a0-128">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="7c3a0-129">userEmail</span><span class="sxs-lookup"><span data-stu-id="7c3a0-129">userEmail</span></span>|<span data-ttu-id="7c3a0-130">String</span><span class="sxs-lookup"><span data-stu-id="7c3a0-130">String</span></span>|<span data-ttu-id="7c3a0-131">记录接受时用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="7c3a0-131">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="7c3a0-132">userId</span><span class="sxs-lookup"><span data-stu-id="7c3a0-132">userId</span></span>|<span data-ttu-id="7c3a0-133">String</span><span class="sxs-lookup"><span data-stu-id="7c3a0-133">String</span></span>|<span data-ttu-id="7c3a0-134">接受协议的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="7c3a0-134">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="7c3a0-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7c3a0-135">userPrincipalName</span></span>|<span data-ttu-id="7c3a0-136">字符串</span><span class="sxs-lookup"><span data-stu-id="7c3a0-136">String</span></span>|<span data-ttu-id="7c3a0-137">记录接受时的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="7c3a0-137">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c3a0-138">关系</span><span class="sxs-lookup"><span data-stu-id="7c3a0-138">Relationships</span></span>
<span data-ttu-id="7c3a0-139">无</span><span class="sxs-lookup"><span data-stu-id="7c3a0-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7c3a0-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c3a0-140">JSON representation</span></span>

<span data-ttu-id="7c3a0-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c3a0-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
  "agreementFileId": "String",
  "agreementId": "String",
  "id": "String (identifier)",
  "recordedDateTime": "String (timestamp)",
  "state": "string",
  "userDisplayName": "String",
  "userEmail": "String",
  "userId": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
