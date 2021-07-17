---
title: externalGroupMember 资源类型
description: 表示 externalGroup 的成员，用于设置对添加到 Microsoft Graph 的外部内容的权限。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e3626c718360982bf79cb9757a13e4b4c01669cd
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467639"
---
# <a name="externalgroupmember-resource-type"></a><span data-ttu-id="a4d1b-103">externalGroupMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4d1b-103">externalGroupMember resource type</span></span>

<span data-ttu-id="a4d1b-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="a4d1b-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4d1b-105">表示[externalGroup](externalconnectors-externalgroup.md)的成员，用于设置对添加到 Microsoft Graph 的外部内容的权限。</span><span class="sxs-lookup"><span data-stu-id="a4d1b-105">Represents a member of an [externalGroup](externalconnectors-externalgroup.md) used to set permissions on external content added to Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="a4d1b-106">方法</span><span class="sxs-lookup"><span data-stu-id="a4d1b-106">Methods</span></span>

| <span data-ttu-id="a4d1b-107">方法</span><span class="sxs-lookup"><span data-stu-id="a4d1b-107">Method</span></span>                                                              | <span data-ttu-id="a4d1b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a4d1b-108">Return type</span></span>         | <span data-ttu-id="a4d1b-109">说明</span><span class="sxs-lookup"><span data-stu-id="a4d1b-109">Description</span></span>                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [<span data-ttu-id="a4d1b-110">创建 externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="a4d1b-110">Create externalGroupMember</span></span>](../api/externalconnectors-externalgroup-post-members.md) | [<span data-ttu-id="a4d1b-111">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="a4d1b-111">externalGroupMember</span></span>](../resources/externalconnectors-externalgroupmember.md) | <span data-ttu-id="a4d1b-112">创建新的 **externalGroupMember** 对象。</span><span class="sxs-lookup"><span data-stu-id="a4d1b-112">Create a new **externalGroupMember** object.</span></span> |
| [<span data-ttu-id="a4d1b-113">删除 externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="a4d1b-113">Delete externalGroupMember</span></span>](../api/externalconnectors-externalgroupmember-delete.md)  | <span data-ttu-id="a4d1b-114">无</span><span class="sxs-lookup"><span data-stu-id="a4d1b-114">None</span></span>                | <span data-ttu-id="a4d1b-115">删除 **externalGroupMember** 对象。</span><span class="sxs-lookup"><span data-stu-id="a4d1b-115">Delete an **externalGroupMember** object.</span></span>   |

## <a name="properties"></a><span data-ttu-id="a4d1b-116">属性</span><span class="sxs-lookup"><span data-stu-id="a4d1b-116">Properties</span></span>

| <span data-ttu-id="a4d1b-117">属性</span><span class="sxs-lookup"><span data-stu-id="a4d1b-117">Property</span></span>       | <span data-ttu-id="a4d1b-118">类型</span><span class="sxs-lookup"><span data-stu-id="a4d1b-118">Type</span></span>                    | <span data-ttu-id="a4d1b-119">说明</span><span class="sxs-lookup"><span data-stu-id="a4d1b-119">Description</span></span>                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| <span data-ttu-id="a4d1b-120">id</span><span class="sxs-lookup"><span data-stu-id="a4d1b-120">id</span></span>             | <span data-ttu-id="a4d1b-121">String</span><span class="sxs-lookup"><span data-stu-id="a4d1b-121">String</span></span>                  | <span data-ttu-id="a4d1b-122">成员的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="a4d1b-122">The unique ID of the member.</span></span> <span data-ttu-id="a4d1b-123">对于用户或组，它将是 objectId Azure Active Directory组，对于外部组，为 **externalGroup** 的 **id** 属性。</span><span class="sxs-lookup"><span data-stu-id="a4d1b-123">It would be the objectId in case of Azure Active Directory users or groups and the **id** property of the **externalGroup** in case of external groups.</span></span>                                    |
| <span data-ttu-id="a4d1b-124">type</span><span class="sxs-lookup"><span data-stu-id="a4d1b-124">type</span></span>           | <span data-ttu-id="a4d1b-125">microsoft.graph.externalConnectors.externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="a4d1b-125">microsoft.graph.externalConnectors.externalGroupMemberType</span></span> | <span data-ttu-id="a4d1b-126">添加到外部组的成员的类型。</span><span class="sxs-lookup"><span data-stu-id="a4d1b-126">The type of member added to the external group.</span></span> <span data-ttu-id="a4d1b-127">可能的值是： `user` 或 `group` 当 **identitySource** 为 时，或者 `azureActiveDirectory` 当 `group` **identitySource** 为 `external` 时。</span><span class="sxs-lookup"><span data-stu-id="a4d1b-127">Possible values are: `user` or `group` when the **identitySource** is `azureActiveDirectory` and just `group` when the **identitySource** is `external`.</span></span> |
| <span data-ttu-id="a4d1b-128">identitySource</span><span class="sxs-lookup"><span data-stu-id="a4d1b-128">identitySource</span></span> | <span data-ttu-id="a4d1b-129">microsoft.graph.externalConnectors.identitySourceType</span><span class="sxs-lookup"><span data-stu-id="a4d1b-129">microsoft.graph.externalConnectors.identitySourceType</span></span>      | <span data-ttu-id="a4d1b-130">成员所属的标识源。</span><span class="sxs-lookup"><span data-stu-id="a4d1b-130">The identity source that the member belongs to.</span></span> <span data-ttu-id="a4d1b-131">可取值为：`azureActiveDirectory`、`external`。</span><span class="sxs-lookup"><span data-stu-id="a4d1b-131">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="relationships"></a><span data-ttu-id="a4d1b-132">关系</span><span class="sxs-lookup"><span data-stu-id="a4d1b-132">Relationships</span></span>

<span data-ttu-id="a4d1b-133">无。</span><span class="sxs-lookup"><span data-stu-id="a4d1b-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4d1b-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4d1b-134">JSON representation</span></span>

<span data-ttu-id="a4d1b-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4d1b-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroupMember",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
