---
title: externalGroup 资源类型
description: 代表在添加到 Microsoft Graph 连接的 externalItems 上用于设置权限的外部组。
author: snlraju-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: c258df9e6f20cf7a19e291fd298ad66345a72949
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193825"
---
# <a name="externalgroup-resource-type"></a><span data-ttu-id="4ff92-103">externalGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ff92-103">externalGroup resource type</span></span>

<span data-ttu-id="4ff92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ff92-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ff92-105">代表一个外部组。</span><span class="sxs-lookup"><span data-stu-id="4ff92-105">Represents an external group.</span></span> <span data-ttu-id="4ff92-106">外部组 (以及 Azure Active Directory users 和 groups) 用于在添加到 Microsoft Graph 连接的 **externalItems** 上设置权限。</span><span class="sxs-lookup"><span data-stu-id="4ff92-106">External groups (along with Azure Active Directory users and groups) are used to set permissions on **externalItems** added to a Microsoft Graph connection.</span></span> <span data-ttu-id="4ff92-107">使用 **externalGroups** 表示非 Azure Active Directory 组或类似组的构造 (例如，) 上的业务单位、团队和子儿子确定对外部数据源中内容的权限。</span><span class="sxs-lookup"><span data-stu-id="4ff92-107">Use **externalGroups** to represent non-Azure Active Directory groups or group-like constructs (such as Business units, Teams, and son on) that determine permission over the content in your external data source.</span></span>

## <a name="methods"></a><span data-ttu-id="4ff92-108">方法</span><span class="sxs-lookup"><span data-stu-id="4ff92-108">Methods</span></span>

|<span data-ttu-id="4ff92-109">方法</span><span class="sxs-lookup"><span data-stu-id="4ff92-109">Method</span></span>|<span data-ttu-id="4ff92-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4ff92-110">Return type</span></span>|<span data-ttu-id="4ff92-111">说明</span><span class="sxs-lookup"><span data-stu-id="4ff92-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4ff92-112">创建 externalGroup</span><span class="sxs-lookup"><span data-stu-id="4ff92-112">Create externalGroup</span></span>](../api/externalconnection-post-groups.md)|[<span data-ttu-id="4ff92-113">externalGroup</span><span class="sxs-lookup"><span data-stu-id="4ff92-113">externalGroup</span></span>](../resources/externalgroup.md)|<span data-ttu-id="4ff92-114">创建新的 **externalGroup** 对象。</span><span class="sxs-lookup"><span data-stu-id="4ff92-114">Create a new **externalGroup** object.</span></span>|
|[<span data-ttu-id="4ff92-115">删除 externalGroup</span><span class="sxs-lookup"><span data-stu-id="4ff92-115">Delete externalGroup</span></span>](../api/externalgroup-delete.md)|<span data-ttu-id="4ff92-116">无</span><span class="sxs-lookup"><span data-stu-id="4ff92-116">None</span></span>|<span data-ttu-id="4ff92-117">删除 **externalGroup** 对象。</span><span class="sxs-lookup"><span data-stu-id="4ff92-117">Delete an **externalGroup** object.</span></span>|
|[<span data-ttu-id="4ff92-118">创建成员</span><span class="sxs-lookup"><span data-stu-id="4ff92-118">Create members</span></span>](../api/externalgroup-post-members.md)|[<span data-ttu-id="4ff92-119">externalGroupMember</span><span class="sxs-lookup"><span data-stu-id="4ff92-119">externalGroupMember</span></span>](../resources/externalgroupmember.md)|<span data-ttu-id="4ff92-120">创建新的 **externalGroupMember** 对象。</span><span class="sxs-lookup"><span data-stu-id="4ff92-120">Create a new **externalGroupMember** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4ff92-121">属性</span><span class="sxs-lookup"><span data-stu-id="4ff92-121">Properties</span></span>

| <span data-ttu-id="4ff92-122">属性</span><span class="sxs-lookup"><span data-stu-id="4ff92-122">Property</span></span>    | <span data-ttu-id="4ff92-123">类型</span><span class="sxs-lookup"><span data-stu-id="4ff92-123">Type</span></span>   | <span data-ttu-id="4ff92-124">说明</span><span class="sxs-lookup"><span data-stu-id="4ff92-124">Description</span></span>                                                                                                              |
|:------------|:-------|:-------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4ff92-125">id</span><span class="sxs-lookup"><span data-stu-id="4ff92-125">id</span></span>          | <span data-ttu-id="4ff92-126">字符串</span><span class="sxs-lookup"><span data-stu-id="4ff92-126">String</span></span> | <span data-ttu-id="4ff92-127">连接中的外部组的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="4ff92-127">The unique ID of the external group within a connection.</span></span> <span data-ttu-id="4ff92-128">它必须是字母数字，最长可为128个字符。</span><span class="sxs-lookup"><span data-stu-id="4ff92-128">It must be alphanumeric and can be up to 128 characters long.</span></span> |
| <span data-ttu-id="4ff92-129">displayName</span><span class="sxs-lookup"><span data-stu-id="4ff92-129">displayName</span></span> | <span data-ttu-id="4ff92-130">字符串</span><span class="sxs-lookup"><span data-stu-id="4ff92-130">String</span></span> | <span data-ttu-id="4ff92-131">外部组的友好名称。</span><span class="sxs-lookup"><span data-stu-id="4ff92-131">The friendly name of the external group.</span></span> <span data-ttu-id="4ff92-132">可选。</span><span class="sxs-lookup"><span data-stu-id="4ff92-132">Optional.</span></span>                                                                       |
| <span data-ttu-id="4ff92-133">说明</span><span class="sxs-lookup"><span data-stu-id="4ff92-133">description</span></span> | <span data-ttu-id="4ff92-134">字符串</span><span class="sxs-lookup"><span data-stu-id="4ff92-134">String</span></span> | <span data-ttu-id="4ff92-135">外部组的说明。</span><span class="sxs-lookup"><span data-stu-id="4ff92-135">The description of the external group.</span></span> <span data-ttu-id="4ff92-136">可选。</span><span class="sxs-lookup"><span data-stu-id="4ff92-136">Optional.</span></span>                                                                         

## <a name="relationships"></a><span data-ttu-id="4ff92-137">关系</span><span class="sxs-lookup"><span data-stu-id="4ff92-137">Relationships</span></span>

| <span data-ttu-id="4ff92-138">关系</span><span class="sxs-lookup"><span data-stu-id="4ff92-138">Relationship</span></span> | <span data-ttu-id="4ff92-139">类型</span><span class="sxs-lookup"><span data-stu-id="4ff92-139">Type</span></span>                                                                  | <span data-ttu-id="4ff92-140">说明</span><span class="sxs-lookup"><span data-stu-id="4ff92-140">Description</span></span>                                               |
|:-------------|:----------------------------------------------------------------------|:----------------------------------------------------------|
| <span data-ttu-id="4ff92-141">成员</span><span class="sxs-lookup"><span data-stu-id="4ff92-141">members</span></span>      | <span data-ttu-id="4ff92-142">[externalGroupMember](../resources/externalgroupmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4ff92-142">[externalGroupMember](../resources/externalgroupmember.md) collection</span></span> | <span data-ttu-id="4ff92-143">添加到 **externalGroup**中的成员。</span><span class="sxs-lookup"><span data-stu-id="4ff92-143">A member added to an **externalGroup**.</span></span> <span data-ttu-id="4ff92-144">你可以将 Azure Active Directory 用户、Azure Active Directory 组或其他 **externalGroups** 添加为成员。</span><span class="sxs-lookup"><span data-stu-id="4ff92-144">You can add Azure Active Directory users, Azure Active Directory groups, or other **externalGroups** as members.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4ff92-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ff92-145">JSON representation</span></span>

<span data-ttu-id="4ff92-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ff92-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalGroup",
  "baseType": "",
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
