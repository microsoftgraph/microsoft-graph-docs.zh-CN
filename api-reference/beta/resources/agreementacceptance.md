---
title: agreementAcceptance 资源类型
description: 表示在受 azure Active Directory (azure AD) 支持的公司自定义使用条款的范围内的用户的当前状态。
localization_priority: Normal
ms.openlocfilehash: 884a6b7dcf4dcc8f00aa927dd9d486c074b64183
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544045"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="396ca-103">agreementAcceptance 资源类型</span><span class="sxs-lookup"><span data-stu-id="396ca-103">agreementAcceptance resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="396ca-104">表示在受 azure Active Directory (azure AD) 支持的公司自定义使用条款的范围内的用户的当前状态。</span><span class="sxs-lookup"><span data-stu-id="396ca-104">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="396ca-105">属性</span><span class="sxs-lookup"><span data-stu-id="396ca-105">Properties</span></span>
| <span data-ttu-id="396ca-106">属性</span><span class="sxs-lookup"><span data-stu-id="396ca-106">Property</span></span>     | <span data-ttu-id="396ca-107">类型</span><span class="sxs-lookup"><span data-stu-id="396ca-107">Type</span></span>        | <span data-ttu-id="396ca-108">说明</span><span class="sxs-lookup"><span data-stu-id="396ca-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="396ca-109">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="396ca-109">agreementFileId</span></span>|<span data-ttu-id="396ca-110">String</span><span class="sxs-lookup"><span data-stu-id="396ca-110">String</span></span>|<span data-ttu-id="396ca-111">用户接受的协议文件的 ID。</span><span class="sxs-lookup"><span data-stu-id="396ca-111">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="396ca-112">agreementId</span><span class="sxs-lookup"><span data-stu-id="396ca-112">agreementId</span></span>|<span data-ttu-id="396ca-113">String</span><span class="sxs-lookup"><span data-stu-id="396ca-113">String</span></span>|<span data-ttu-id="396ca-114">协议的 ID。</span><span class="sxs-lookup"><span data-stu-id="396ca-114">ID of the agreement.</span></span>|
|<span data-ttu-id="396ca-115">id</span><span class="sxs-lookup"><span data-stu-id="396ca-115">id</span></span>|<span data-ttu-id="396ca-116">String</span><span class="sxs-lookup"><span data-stu-id="396ca-116">String</span></span>| <span data-ttu-id="396ca-117">只读。</span><span class="sxs-lookup"><span data-stu-id="396ca-117">Read-only.</span></span>|
|<span data-ttu-id="396ca-118">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="396ca-118">recordedDateTime</span></span>|<span data-ttu-id="396ca-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="396ca-119">DateTimeOffset</span></span>|<span data-ttu-id="396ca-p101">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="396ca-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="396ca-122">state</span><span class="sxs-lookup"><span data-stu-id="396ca-122">state</span></span>|<span data-ttu-id="396ca-123">string</span><span class="sxs-lookup"><span data-stu-id="396ca-123">string</span></span>| <span data-ttu-id="396ca-124">可取值为：`accepted`、`declined`。</span><span class="sxs-lookup"><span data-stu-id="396ca-124">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="396ca-125">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="396ca-125">userDisplayName</span></span>|<span data-ttu-id="396ca-126">String</span><span class="sxs-lookup"><span data-stu-id="396ca-126">String</span></span>|<span data-ttu-id="396ca-127">记录接受时的用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="396ca-127">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="396ca-128">userEmail</span><span class="sxs-lookup"><span data-stu-id="396ca-128">userEmail</span></span>|<span data-ttu-id="396ca-129">String</span><span class="sxs-lookup"><span data-stu-id="396ca-129">String</span></span>|<span data-ttu-id="396ca-130">记录接受时用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="396ca-130">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="396ca-131">userId</span><span class="sxs-lookup"><span data-stu-id="396ca-131">userId</span></span>|<span data-ttu-id="396ca-132">String</span><span class="sxs-lookup"><span data-stu-id="396ca-132">String</span></span>|<span data-ttu-id="396ca-133">接受协议的用户的 ID。</span><span class="sxs-lookup"><span data-stu-id="396ca-133">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="396ca-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="396ca-134">userPrincipalName</span></span>|<span data-ttu-id="396ca-135">String</span><span class="sxs-lookup"><span data-stu-id="396ca-135">String</span></span>|<span data-ttu-id="396ca-136">记录接受时的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="396ca-136">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="396ca-137">关系</span><span class="sxs-lookup"><span data-stu-id="396ca-137">Relationships</span></span>
<span data-ttu-id="396ca-138">无</span><span class="sxs-lookup"><span data-stu-id="396ca-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="396ca-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="396ca-139">JSON representation</span></span>

<span data-ttu-id="396ca-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="396ca-140">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementacceptance.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
