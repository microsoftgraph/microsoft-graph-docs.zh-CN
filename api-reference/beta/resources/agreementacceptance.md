---
title: agreementAcceptance 资源类型
description: 表示的公司的可自定义使用条款由 Azure Active Directory (Azure AD) 的范围内的用户的当前状态。
ms.openlocfilehash: 23221fe88a65b003c8d26aca99eaf1f03d935722
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041477"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="179b4-103">agreementAcceptance 资源类型</span><span class="sxs-lookup"><span data-stu-id="179b4-103">agreementAcceptance resource type</span></span>

> <span data-ttu-id="179b4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="179b4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="179b4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="179b4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="179b4-106">表示的公司的可自定义使用条款由 Azure Active Directory (Azure AD) 的范围内的用户的当前状态。</span><span class="sxs-lookup"><span data-stu-id="179b4-106">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="179b4-107">属性</span><span class="sxs-lookup"><span data-stu-id="179b4-107">Properties</span></span>
| <span data-ttu-id="179b4-108">属性</span><span class="sxs-lookup"><span data-stu-id="179b4-108">Property</span></span>     | <span data-ttu-id="179b4-109">类型</span><span class="sxs-lookup"><span data-stu-id="179b4-109">Type</span></span>        | <span data-ttu-id="179b4-110">说明</span><span class="sxs-lookup"><span data-stu-id="179b4-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="179b4-111">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="179b4-111">agreementFileId</span></span>|<span data-ttu-id="179b4-112">字符串</span><span class="sxs-lookup"><span data-stu-id="179b4-112">String</span></span>|<span data-ttu-id="179b4-113">由用户接受协议文件的 ID。</span><span class="sxs-lookup"><span data-stu-id="179b4-113">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="179b4-114">agreementId</span><span class="sxs-lookup"><span data-stu-id="179b4-114">agreementId</span></span>|<span data-ttu-id="179b4-115">字符串</span><span class="sxs-lookup"><span data-stu-id="179b4-115">String</span></span>|<span data-ttu-id="179b4-116">协议中的 ID。</span><span class="sxs-lookup"><span data-stu-id="179b4-116">ID of the agreement.</span></span>|
|<span data-ttu-id="179b4-117">id</span><span class="sxs-lookup"><span data-stu-id="179b4-117">id</span></span>|<span data-ttu-id="179b4-118">String</span><span class="sxs-lookup"><span data-stu-id="179b4-118">String</span></span>| <span data-ttu-id="179b4-119">只读。</span><span class="sxs-lookup"><span data-stu-id="179b4-119">Read-only.</span></span>|
|<span data-ttu-id="179b4-120">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="179b4-120">recordedDateTime</span></span>|<span data-ttu-id="179b4-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="179b4-121">DateTimeOffset</span></span>|<span data-ttu-id="179b4-p102">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="179b4-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="179b4-124">state</span><span class="sxs-lookup"><span data-stu-id="179b4-124">state</span></span>|<span data-ttu-id="179b4-125">string</span><span class="sxs-lookup"><span data-stu-id="179b4-125">string</span></span>| <span data-ttu-id="179b4-126">可取值为：`accepted`、`declined`。</span><span class="sxs-lookup"><span data-stu-id="179b4-126">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="179b4-127">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="179b4-127">userDisplayName</span></span>|<span data-ttu-id="179b4-128">String</span><span class="sxs-lookup"><span data-stu-id="179b4-128">String</span></span>|<span data-ttu-id="179b4-129">当记录被接受的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="179b4-129">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="179b4-130">userEmail</span><span class="sxs-lookup"><span data-stu-id="179b4-130">userEmail</span></span>|<span data-ttu-id="179b4-131">String</span><span class="sxs-lookup"><span data-stu-id="179b4-131">String</span></span>|<span data-ttu-id="179b4-132">当记录被接受的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="179b4-132">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="179b4-133">userId</span><span class="sxs-lookup"><span data-stu-id="179b4-133">userId</span></span>|<span data-ttu-id="179b4-134">String</span><span class="sxs-lookup"><span data-stu-id="179b4-134">String</span></span>|<span data-ttu-id="179b4-135">接受此协议的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="179b4-135">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="179b4-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="179b4-136">userPrincipalName</span></span>|<span data-ttu-id="179b4-137">字符串</span><span class="sxs-lookup"><span data-stu-id="179b4-137">String</span></span>|<span data-ttu-id="179b4-138">当记录被接受用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="179b4-138">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="179b4-139">Relationships</span><span class="sxs-lookup"><span data-stu-id="179b4-139">Relationships</span></span>
<span data-ttu-id="179b4-140">无</span><span class="sxs-lookup"><span data-stu-id="179b4-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="179b4-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="179b4-141">JSON representation</span></span>

<span data-ttu-id="179b4-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="179b4-142">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
