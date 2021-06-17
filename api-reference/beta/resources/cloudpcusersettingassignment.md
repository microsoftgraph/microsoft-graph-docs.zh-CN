---
title: cloudPcUserSettingAssignment 资源类型
description: 表示定义的用户设置分配集合。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 704142ce266a826606b6c32b209d69d052d1a3c9
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993683"
---
# <a name="cloudpcusersettingassignment--resource-type"></a><span data-ttu-id="804a2-103">cloudPcUserSettingAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="804a2-103">cloudPcUserSettingAssignment  resource type</span></span>

<span data-ttu-id="804a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="804a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="804a2-105">表示定义的用户设置分配集合。</span><span class="sxs-lookup"><span data-stu-id="804a2-105">Represents a defined collection of user setting assignments.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="804a2-106">属性</span><span class="sxs-lookup"><span data-stu-id="804a2-106">Properties</span></span>

|<span data-ttu-id="804a2-107">属性</span><span class="sxs-lookup"><span data-stu-id="804a2-107">Property</span></span>|<span data-ttu-id="804a2-108">类型</span><span class="sxs-lookup"><span data-stu-id="804a2-108">Type</span></span>|<span data-ttu-id="804a2-109">说明</span><span class="sxs-lookup"><span data-stu-id="804a2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="804a2-110">id</span><span class="sxs-lookup"><span data-stu-id="804a2-110">id</span></span>|<span data-ttu-id="804a2-111">String</span><span class="sxs-lookup"><span data-stu-id="804a2-111">String</span></span>|<span data-ttu-id="804a2-112">用户设置分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="804a2-112">Unique Identifier for the user setting assignment.</span></span> <span data-ttu-id="804a2-113">只读。</span><span class="sxs-lookup"><span data-stu-id="804a2-113">Read-only.</span></span> <span data-ttu-id="804a2-114">如果 `target` 为用户组，则 ID 具有以下结构：{policyID}_{groupID}。</span><span class="sxs-lookup"><span data-stu-id="804a2-114">If `target` is a user group, the ID has this structure: {policyID}_{groupID}.</span></span>|
|<span data-ttu-id="804a2-115">target</span><span class="sxs-lookup"><span data-stu-id="804a2-115">target</span></span>|[<span data-ttu-id="804a2-116">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="804a2-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="804a2-117">用户设置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="804a2-117">The assignment target for the user setting.</span></span> <span data-ttu-id="804a2-118">目前，用户设置支持的唯一目标为用户组。</span><span class="sxs-lookup"><span data-stu-id="804a2-118">Currently, the only target supported for user setting is a user group.</span></span>|
|<span data-ttu-id="804a2-119">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="804a2-119">createdDateTime</span></span>|<span data-ttu-id="804a2-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="804a2-120">DateTimeOffset</span></span>|<span data-ttu-id="804a2-121">创建此工作分配的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="804a2-121">The date and time this assignment was created.</span></span> <span data-ttu-id="804a2-122">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="804a2-122">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="804a2-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="804a2-123">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="804a2-124">关系</span><span class="sxs-lookup"><span data-stu-id="804a2-124">Relationships</span></span>

<span data-ttu-id="804a2-125">无。</span><span class="sxs-lookup"><span data-stu-id="804a2-125">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="804a2-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="804a2-126">JSON representation</span></span>
<span data-ttu-id="804a2-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="804a2-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcUserSettingAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cloudPcUserSettingAssignment",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.cloudPcManagementAssignmentTarget"
  }
}
```
