---
title: cloudPcUserSettingAssignment 资源类型
description: 表示定义的用户设置分配集合。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: db97ff52ff8eb7ca1ef52563d577d5076273d859
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082179"
---
# <a name="cloudpcusersettingassignment--resource-type"></a><span data-ttu-id="66376-103">cloudPcUserSettingAssignment 资源类型</span><span class="sxs-lookup"><span data-stu-id="66376-103">cloudPcUserSettingAssignment  resource type</span></span>

<span data-ttu-id="66376-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66376-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66376-105">表示定义的用户设置分配集合。</span><span class="sxs-lookup"><span data-stu-id="66376-105">Represents a defined collection of user setting assignments.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="66376-106">属性</span><span class="sxs-lookup"><span data-stu-id="66376-106">Properties</span></span>

|<span data-ttu-id="66376-107">属性</span><span class="sxs-lookup"><span data-stu-id="66376-107">Property</span></span>|<span data-ttu-id="66376-108">类型</span><span class="sxs-lookup"><span data-stu-id="66376-108">Type</span></span>|<span data-ttu-id="66376-109">说明</span><span class="sxs-lookup"><span data-stu-id="66376-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66376-110">id</span><span class="sxs-lookup"><span data-stu-id="66376-110">id</span></span>|<span data-ttu-id="66376-111">String</span><span class="sxs-lookup"><span data-stu-id="66376-111">String</span></span>|<span data-ttu-id="66376-112">用户设置分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="66376-112">Unique Identifier for the user setting assignment.</span></span> <span data-ttu-id="66376-113">只读。</span><span class="sxs-lookup"><span data-stu-id="66376-113">Read-only.</span></span> <span data-ttu-id="66376-114">如果 `target` 为用户组，则 ID 具有以下结构：{policyID} \_ {groupID}。</span><span class="sxs-lookup"><span data-stu-id="66376-114">If `target` is a user group, the ID has this structure: {policyID}\_{groupID}.</span></span>|
|<span data-ttu-id="66376-115">target</span><span class="sxs-lookup"><span data-stu-id="66376-115">target</span></span>|[<span data-ttu-id="66376-116">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="66376-116">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="66376-117">用户设置的分配目标。</span><span class="sxs-lookup"><span data-stu-id="66376-117">The assignment target for the user setting.</span></span> <span data-ttu-id="66376-118">目前，此用户设置支持的唯一目标为用户组。</span><span class="sxs-lookup"><span data-stu-id="66376-118">Currently, the only target supported for this user setting is a user group.</span></span> <span data-ttu-id="66376-119">有关详细信息，请参阅 [cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md)。</span><span class="sxs-lookup"><span data-stu-id="66376-119">For details, see [cloudPcManagementGroupAssignmentTarget](cloudpcmanagementgroupassignmenttarget.md).</span></span>|
|<span data-ttu-id="66376-120">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66376-120">createdDateTime</span></span>|<span data-ttu-id="66376-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66376-121">DateTimeOffset</span></span>|<span data-ttu-id="66376-122">创建此工作分配的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="66376-122">The date and time this assignment was created.</span></span> <span data-ttu-id="66376-123">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="66376-123">The Timestamp type represents the date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="66376-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示："2014-01-01T00：00：00Z"。</span><span class="sxs-lookup"><span data-stu-id="66376-124">For example, midnight UTC on Jan 1, 2014 looks like this: '2014-01-01T00:00:00Z'.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="66376-125">关系</span><span class="sxs-lookup"><span data-stu-id="66376-125">Relationships</span></span>

<span data-ttu-id="66376-126">无。</span><span class="sxs-lookup"><span data-stu-id="66376-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66376-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="66376-127">JSON representation</span></span>
<span data-ttu-id="66376-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66376-128">The following is a JSON representation of the resource.</span></span>
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
