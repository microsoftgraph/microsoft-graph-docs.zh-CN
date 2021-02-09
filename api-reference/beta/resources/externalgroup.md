---
title: externalGroup 资源类型
description: 表示一个外部组，用于设置对添加到 Microsoft Graph 连接的外部项目的权限。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2e9d8e3a605f1c3df39b13607f82e7541d59e62e
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161700"
---
# <a name="externalgroup-resource-type"></a><span data-ttu-id="cd9f4-103">externalGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd9f4-103">externalGroup resource type</span></span>

<span data-ttu-id="cd9f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd9f4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd9f4-105">表示外部组。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-105">Represents an external group.</span></span> <span data-ttu-id="cd9f4-106">外部组 (Azure Active Directory 用户和组) 用于设置对添加到 Microsoft Graph 连接 **的外部** 项目的权限。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-106">External groups (along with Azure Active Directory users and groups) are used to set permissions on **externalItems** added to a Microsoft Graph connection.</span></span> <span data-ttu-id="cd9f4-107">使用 **externalGroups** 表示非 Azure Active Directory 组或类似组 (例如) 上的业务单位、Teams 和子级，这些构造可确定对外部数据源中内容的权限。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-107">Use **externalGroups** to represent non-Azure Active Directory groups or group-like constructs (such as Business units, Teams, and son on) that determine permission over the content in your external data source.</span></span>

## <a name="methods"></a><span data-ttu-id="cd9f4-108">方法</span><span class="sxs-lookup"><span data-stu-id="cd9f4-108">Methods</span></span>

|<span data-ttu-id="cd9f4-109">方法</span><span class="sxs-lookup"><span data-stu-id="cd9f4-109">Method</span></span>|<span data-ttu-id="cd9f4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cd9f4-110">Return type</span></span>|<span data-ttu-id="cd9f4-111">说明</span><span class="sxs-lookup"><span data-stu-id="cd9f4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cd9f4-112">创建 externalGroup</span><span class="sxs-lookup"><span data-stu-id="cd9f4-112">Create externalGroup</span></span>](../api/externalconnection-post-groups.md)|[<span data-ttu-id="cd9f4-113">externalGroup</span><span class="sxs-lookup"><span data-stu-id="cd9f4-113">externalGroup</span></span>](../resources/externalgroup.md)|<span data-ttu-id="cd9f4-114">创建新的 **externalGroup** 对象。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-114">Create a new **externalGroup** object.</span></span>|
|[<span data-ttu-id="cd9f4-115">删除 externalGroup</span><span class="sxs-lookup"><span data-stu-id="cd9f4-115">Delete externalGroup</span></span>](../api/externalgroup-delete.md)|<span data-ttu-id="cd9f4-116">无</span><span class="sxs-lookup"><span data-stu-id="cd9f4-116">None</span></span>|<span data-ttu-id="cd9f4-117">删除 **externalGroup** 对象。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-117">Delete an **externalGroup** object.</span></span>|
|[<span data-ttu-id="cd9f4-118">创建成员</span><span class="sxs-lookup"><span data-stu-id="cd9f4-118">Create members</span></span>](../api/externalgroup-post-members.md)|[<span data-ttu-id="cd9f4-119">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="cd9f4-119">externalGroupMember</span></span>](../resources/externalgroupmember.md)|<span data-ttu-id="cd9f4-120">创建新的 **externalGroupMember** 对象。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-120">Create a new **externalGroupMember** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd9f4-121">属性</span><span class="sxs-lookup"><span data-stu-id="cd9f4-121">Properties</span></span>

| <span data-ttu-id="cd9f4-122">属性</span><span class="sxs-lookup"><span data-stu-id="cd9f4-122">Property</span></span>    | <span data-ttu-id="cd9f4-123">类型</span><span class="sxs-lookup"><span data-stu-id="cd9f4-123">Type</span></span>   | <span data-ttu-id="cd9f4-124">说明</span><span class="sxs-lookup"><span data-stu-id="cd9f4-124">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cd9f4-125">id</span><span class="sxs-lookup"><span data-stu-id="cd9f4-125">id</span></span>          | <span data-ttu-id="cd9f4-126">String</span><span class="sxs-lookup"><span data-stu-id="cd9f4-126">String</span></span> | <span data-ttu-id="cd9f4-127">连接内外部组的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-127">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="cd9f4-128">它必须是字母数字，并且最多为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-128">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="cd9f4-129">displayName</span><span class="sxs-lookup"><span data-stu-id="cd9f4-129">displayName</span></span> | <span data-ttu-id="cd9f4-130">String</span><span class="sxs-lookup"><span data-stu-id="cd9f4-130">String</span></span> | <span data-ttu-id="cd9f4-131">外部组的友好名称。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-131">The friendly name of the external group.</span></span> <span data-ttu-id="cd9f4-132">可选。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-132">Optional.</span></span>                                                                       |
| <span data-ttu-id="cd9f4-133">说明</span><span class="sxs-lookup"><span data-stu-id="cd9f4-133">description</span></span> | <span data-ttu-id="cd9f4-134">String</span><span class="sxs-lookup"><span data-stu-id="cd9f4-134">String</span></span> | <span data-ttu-id="cd9f4-135">外部组的说明。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-135">The description of the external group.</span></span> <span data-ttu-id="cd9f4-136">可选。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-136">Optional.</span></span>                                                                         

## <a name="relationships"></a><span data-ttu-id="cd9f4-137">关系</span><span class="sxs-lookup"><span data-stu-id="cd9f4-137">Relationships</span></span>

| <span data-ttu-id="cd9f4-138">关系</span><span class="sxs-lookup"><span data-stu-id="cd9f4-138">Relationship</span></span> | <span data-ttu-id="cd9f4-139">类型</span><span class="sxs-lookup"><span data-stu-id="cd9f4-139">Type</span></span>                                                                  | <span data-ttu-id="cd9f4-140">说明</span><span class="sxs-lookup"><span data-stu-id="cd9f4-140">Description</span></span>                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="cd9f4-141">成员</span><span class="sxs-lookup"><span data-stu-id="cd9f4-141">members</span></span>      | <span data-ttu-id="cd9f4-142">[externalGroupMember](../resources/externalgroupmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cd9f4-142">[externalGroupMember](../resources/externalgroupmember.md) collection</span></span> | <span data-ttu-id="cd9f4-143">添加到 **externalGroup 的成员**。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-143">A member added to an **externalGroup**.</span></span> <span data-ttu-id="cd9f4-144">可以将 Azure Active Directory 用户、Azure Active Directory 组或其他 **外部组** 添加为成员。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-144">You can add Azure Active Directory users, Azure Active Directory groups, or other **externalGroups** as members.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="cd9f4-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd9f4-145">JSON representation</span></span>

<span data-ttu-id="cd9f4-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd9f4-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroup",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.externalGroup",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```
