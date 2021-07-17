---
title: externalGroup 资源类型
description: 表示一个外部组，用于对添加到 Microsoft Graph外部项目设置权限。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3f0c6adbd47d1823b82e19d3fb9a352e26391da9
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467643"
---
# <a name="externalgroup-resource-type"></a><span data-ttu-id="2cfa9-103">externalGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="2cfa9-103">externalGroup resource type</span></span>

<span data-ttu-id="2cfa9-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="2cfa9-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cfa9-105">表示外部组。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-105">Represents an external group.</span></span> <span data-ttu-id="2cfa9-106">外部 (组Azure Active Directory用户和组) 用于设置对添加到 Microsoft Graph 连接的外部项的权限。 </span><span class="sxs-lookup"><span data-stu-id="2cfa9-106">External groups (along with Azure Active Directory users and groups) are used to set permissions on **externalItems** added to a Microsoft Graph connection.</span></span> <span data-ttu-id="2cfa9-107">使用 **externalGroups** 表示非 Azure Active Directory 组或类似组的构造 (如) 上的业务单位、Teams 和 son，这些构造可确定对外部数据源中内容的权限。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-107">Use **externalGroups** to represent non-Azure Active Directory groups or group-like constructs (such as Business units, Teams, and son on) that determine permission over the content in your external data source.</span></span>

## <a name="methods"></a><span data-ttu-id="2cfa9-108">方法</span><span class="sxs-lookup"><span data-stu-id="2cfa9-108">Methods</span></span>

|<span data-ttu-id="2cfa9-109">方法</span><span class="sxs-lookup"><span data-stu-id="2cfa9-109">Method</span></span>|<span data-ttu-id="2cfa9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2cfa9-110">Return type</span></span>|<span data-ttu-id="2cfa9-111">说明</span><span class="sxs-lookup"><span data-stu-id="2cfa9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2cfa9-112">创建 externalGroup</span><span class="sxs-lookup"><span data-stu-id="2cfa9-112">Create externalGroup</span></span>](../api/externalconnectors-externalconnection-post-groups.md)|[<span data-ttu-id="2cfa9-113">microsoft.graph.externalConnectors.externalGroup</span><span class="sxs-lookup"><span data-stu-id="2cfa9-113">microsoft.graph.externalConnectors.externalGroup</span></span>](../resources/externalconnectors-externalgroup.md)|<span data-ttu-id="2cfa9-114">创建新的 **externalGroup** 对象。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-114">Create a new **externalGroup** object.</span></span>|
|[<span data-ttu-id="2cfa9-115">删除 externalGroup</span><span class="sxs-lookup"><span data-stu-id="2cfa9-115">Delete externalGroup</span></span>](../api/externalconnectors-externalgroup-delete.md)|<span data-ttu-id="2cfa9-116">无</span><span class="sxs-lookup"><span data-stu-id="2cfa9-116">None</span></span>|<span data-ttu-id="2cfa9-117">删除 **externalGroup** 对象。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-117">Delete an **externalGroup** object.</span></span>|
|[<span data-ttu-id="2cfa9-118">创建成员</span><span class="sxs-lookup"><span data-stu-id="2cfa9-118">Create members</span></span>](../api/externalconnectors-externalgroup-post-members.md)|[<span data-ttu-id="2cfa9-119">microsoft.graph.externalConnectors.externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="2cfa9-119">microsoft.graph.externalConnectors.externalGroupMember</span></span>](../resources/externalconnectors-externalgroupmember.md)|<span data-ttu-id="2cfa9-120">创建新的 **externalGroupMember** 对象。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-120">Create a new **externalGroupMember** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2cfa9-121">属性</span><span class="sxs-lookup"><span data-stu-id="2cfa9-121">Properties</span></span>

| <span data-ttu-id="2cfa9-122">属性</span><span class="sxs-lookup"><span data-stu-id="2cfa9-122">Property</span></span>    | <span data-ttu-id="2cfa9-123">类型</span><span class="sxs-lookup"><span data-stu-id="2cfa9-123">Type</span></span>   | <span data-ttu-id="2cfa9-124">说明</span><span class="sxs-lookup"><span data-stu-id="2cfa9-124">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2cfa9-125">id</span><span class="sxs-lookup"><span data-stu-id="2cfa9-125">id</span></span>          | <span data-ttu-id="2cfa9-126">String</span><span class="sxs-lookup"><span data-stu-id="2cfa9-126">String</span></span> | <span data-ttu-id="2cfa9-127">连接内外部组的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-127">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="2cfa9-128">它必须是字母数字，并且最多为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-128">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="2cfa9-129">displayName</span><span class="sxs-lookup"><span data-stu-id="2cfa9-129">displayName</span></span> | <span data-ttu-id="2cfa9-130">String</span><span class="sxs-lookup"><span data-stu-id="2cfa9-130">String</span></span> | <span data-ttu-id="2cfa9-131">外部组的友好名称。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-131">The friendly name of the external group.</span></span> <span data-ttu-id="2cfa9-132">可选。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-132">Optional.</span></span>                                                                       |
| <span data-ttu-id="2cfa9-133">说明</span><span class="sxs-lookup"><span data-stu-id="2cfa9-133">description</span></span> | <span data-ttu-id="2cfa9-134">String</span><span class="sxs-lookup"><span data-stu-id="2cfa9-134">String</span></span> | <span data-ttu-id="2cfa9-135">外部组的说明。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-135">The description of the external group.</span></span> <span data-ttu-id="2cfa9-136">可选。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-136">Optional.</span></span>                                                                         

## <a name="relationships"></a><span data-ttu-id="2cfa9-137">关系</span><span class="sxs-lookup"><span data-stu-id="2cfa9-137">Relationships</span></span>

| <span data-ttu-id="2cfa9-138">关系</span><span class="sxs-lookup"><span data-stu-id="2cfa9-138">Relationship</span></span> | <span data-ttu-id="2cfa9-139">类型</span><span class="sxs-lookup"><span data-stu-id="2cfa9-139">Type</span></span>                                                                  | <span data-ttu-id="2cfa9-140">说明</span><span class="sxs-lookup"><span data-stu-id="2cfa9-140">Description</span></span>                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="2cfa9-141">成员</span><span class="sxs-lookup"><span data-stu-id="2cfa9-141">members</span></span>      | <span data-ttu-id="2cfa9-142">[microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2cfa9-142">[microsoft.graph.externalConnectors.externalGroupMember](../resources/externalconnectors-externalgroupmember.md) collection</span></span> | <span data-ttu-id="2cfa9-143">添加到 **externalGroup 的成员**。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-143">A member added to an **externalGroup**.</span></span> <span data-ttu-id="2cfa9-144">可以将用户Azure Active Directory组Azure Active Directory其他 **externalGroups 添加** 为成员。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-144">You can add Azure Active Directory users, Azure Active Directory groups, or other **externalGroups** as members.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2cfa9-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cfa9-145">JSON representation</span></span>

<span data-ttu-id="2cfa9-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2cfa9-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.externalGroup",
  "openType": false
}
-->

``` json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```
