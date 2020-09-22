---
title: externalGroupMember 资源类型
description: 表示用于对添加到 Microsoft Graph 的外部内容设置权限的 externalGroup 的成员。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 19b5c5094501215cc3ffd3e852ba6ca427807988
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193824"
---
# <a name="externalgroupmember-resource-type"></a><span data-ttu-id="f0afc-103">externalGroupMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0afc-103">externalGroupMember resource type</span></span>

<span data-ttu-id="f0afc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0afc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0afc-105">表示用于对添加到 Microsoft Graph 的外部内容设置权限的 [externalGroup](externalgroup.md) 的成员。</span><span class="sxs-lookup"><span data-stu-id="f0afc-105">Represents a member of an [externalGroup](externalgroup.md) used to set permissions on external content added to Microsoft Graph.</span></span>

## <a name="methods"></a><span data-ttu-id="f0afc-106">方法</span><span class="sxs-lookup"><span data-stu-id="f0afc-106">Methods</span></span>

| <span data-ttu-id="f0afc-107">方法</span><span class="sxs-lookup"><span data-stu-id="f0afc-107">Method</span></span>                                                              | <span data-ttu-id="f0afc-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f0afc-108">Return type</span></span>         | <span data-ttu-id="f0afc-109">说明</span><span class="sxs-lookup"><span data-stu-id="f0afc-109">Description</span></span>                              |
|:--------------------------------------------------------------------|:--------------------|:-----------------------------------------|
| [<span data-ttu-id="f0afc-110">创建 externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="f0afc-110">Create externalGroupMember</span></span>](../api/externalgroup-post-members.md) | <span data-ttu-id="f0afc-111">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="f0afc-111">externalGroupMember</span></span> | <span data-ttu-id="f0afc-112">创建新的 **externalGroupMember** 对象。</span><span class="sxs-lookup"><span data-stu-id="f0afc-112">Create a new **externalGroupMember** object.</span></span> |
| [<span data-ttu-id="f0afc-113">删除 externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="f0afc-113">Delete externalGroupMember</span></span>](../api/externalgroupmember-delete.md)  | <span data-ttu-id="f0afc-114">无</span><span class="sxs-lookup"><span data-stu-id="f0afc-114">None</span></span>                | <span data-ttu-id="f0afc-115">删除 **externalGroupMember** 对象。</span><span class="sxs-lookup"><span data-stu-id="f0afc-115">Delete an **externalGroupMember** object.</span></span>   |

## <a name="properties"></a><span data-ttu-id="f0afc-116">属性</span><span class="sxs-lookup"><span data-stu-id="f0afc-116">Properties</span></span>

| <span data-ttu-id="f0afc-117">属性</span><span class="sxs-lookup"><span data-stu-id="f0afc-117">Property</span></span>       | <span data-ttu-id="f0afc-118">类型</span><span class="sxs-lookup"><span data-stu-id="f0afc-118">Type</span></span>                    | <span data-ttu-id="f0afc-119">说明</span><span class="sxs-lookup"><span data-stu-id="f0afc-119">Description</span></span>                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| <span data-ttu-id="f0afc-120">id</span><span class="sxs-lookup"><span data-stu-id="f0afc-120">id</span></span>             | <span data-ttu-id="f0afc-121">字符串</span><span class="sxs-lookup"><span data-stu-id="f0afc-121">String</span></span>                  | <span data-ttu-id="f0afc-122">成员的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="f0afc-122">The unique ID of the member.</span></span> <span data-ttu-id="f0afc-123">当 Azure Active Directory 用户或组以及外部组的 **id** 属性为 **externalGroup** 时，它就是相应的 objectId。</span><span class="sxs-lookup"><span data-stu-id="f0afc-123">It would be the objectId in case of Azure Active Directory users or groups and the **id** property of the **externalGroup** in case of external groups.</span></span>                                    |
| <span data-ttu-id="f0afc-124">type</span><span class="sxs-lookup"><span data-stu-id="f0afc-124">type</span></span>           | <span data-ttu-id="f0afc-125">externalGroupMemberType</span><span class="sxs-lookup"><span data-stu-id="f0afc-125">externalGroupMemberType</span></span> | <span data-ttu-id="f0afc-126">添加到外部组的成员类型。</span><span class="sxs-lookup"><span data-stu-id="f0afc-126">The type of member added to the external group.</span></span> <span data-ttu-id="f0afc-127">可能的值为： `user` 或者 `group` 当 **identitySource** 是 `azureActiveDirectory` `group` **identitySource** 时， `external` 则为。</span><span class="sxs-lookup"><span data-stu-id="f0afc-127">Possible values are: `user` or `group` when the **identitySource** is `azureActiveDirectory` and just `group` when the **identitySource** is `external`.</span></span> |
| <span data-ttu-id="f0afc-128">identitySource</span><span class="sxs-lookup"><span data-stu-id="f0afc-128">identitySource</span></span> | <span data-ttu-id="f0afc-129">identitySourceType</span><span class="sxs-lookup"><span data-stu-id="f0afc-129">identitySourceType</span></span>      | <span data-ttu-id="f0afc-130">成员所属的标识源。</span><span class="sxs-lookup"><span data-stu-id="f0afc-130">The identity source that the member belongs to.</span></span> <span data-ttu-id="f0afc-131">可取值为：`azureActiveDirectory`、`external`。</span><span class="sxs-lookup"><span data-stu-id="f0afc-131">Possible values are: `azureActiveDirectory`, `external`.</span></span>                                                                                         |

## <a name="relationships"></a><span data-ttu-id="f0afc-132">关系</span><span class="sxs-lookup"><span data-stu-id="f0afc-132">Relationships</span></span>

<span data-ttu-id="f0afc-133">无。</span><span class="sxs-lookup"><span data-stu-id="f0afc-133">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0afc-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0afc-134">JSON representation</span></span>

<span data-ttu-id="f0afc-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0afc-135">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroupMember",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroupMember",
  "id": "String (identifier)",
  "type": "String",
  "identitySource": "String"
}
```
