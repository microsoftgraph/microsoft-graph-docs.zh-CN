---
title: organizationSettings 资源类型
description: 包含适用于组织或其内的用户对象的设置。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 80b7272915cd6f9dbfc381aa93a32896e2eaf3f5
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050999"
---
# <a name="organizationsettings-resource-type"></a><span data-ttu-id="35713-103">organizationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="35713-103">organizationSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35713-104">包含适用于[组织](organization.md)或应应用于组织中的[用户](user.md)对象的设置。</span><span class="sxs-lookup"><span data-stu-id="35713-104">Contains settings that are applicable to the [organization](organization.md) or that should be applied to [user](user.md) objects within an organization.</span></span>

## <a name="methods"></a><span data-ttu-id="35713-105">方法</span><span class="sxs-lookup"><span data-stu-id="35713-105">Methods</span></span>

| <span data-ttu-id="35713-106">方法</span><span class="sxs-lookup"><span data-stu-id="35713-106">Method</span></span>       | <span data-ttu-id="35713-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="35713-107">Return Type</span></span> | <span data-ttu-id="35713-108">说明</span><span class="sxs-lookup"><span data-stu-id="35713-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="35713-109">获取组织设置</span><span class="sxs-lookup"><span data-stu-id="35713-109">Get organization settings</span></span>](../api/organizationsettings-get.md) | [<span data-ttu-id="35713-110">organizationSettings</span><span class="sxs-lookup"><span data-stu-id="35713-110">organizationSettings</span></span>](organizationsettings.md) | <span data-ttu-id="35713-111">读取组织设置对象。</span><span class="sxs-lookup"><span data-stu-id="35713-111">Read the organization settings object.</span></span> |
| [<span data-ttu-id="35713-112">创建 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="35713-112">Create profileCardProperty</span></span>](../api/organizationsettings-post-profilecardproperties.md) | [<span data-ttu-id="35713-113">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="35713-113">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="35713-114">通过发布到 profileCardProperties 集合创建新的 profileCardProperty。</span><span class="sxs-lookup"><span data-stu-id="35713-114">Create a new profileCardProperty by posting to the profileCardProperties collection.</span></span> |
| [<span data-ttu-id="35713-115">列出 profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="35713-115">List profileCardProperties</span></span>](../api/organizationsettings-list-profilecardproperties.md) | <span data-ttu-id="35713-116">[profileCardProperty](profilecardproperty.md)集合</span><span class="sxs-lookup"><span data-stu-id="35713-116">[profileCardProperty](profilecardproperty.md) collection</span></span> | <span data-ttu-id="35713-117">获取 profileCardProperty 对象集合。</span><span class="sxs-lookup"><span data-stu-id="35713-117">Get a profileCardProperty object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="35713-118">属性</span><span class="sxs-lookup"><span data-stu-id="35713-118">Properties</span></span>

<span data-ttu-id="35713-119">无。</span><span class="sxs-lookup"><span data-stu-id="35713-119">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="35713-120">关系</span><span class="sxs-lookup"><span data-stu-id="35713-120">Relationships</span></span>

| <span data-ttu-id="35713-121">关系</span><span class="sxs-lookup"><span data-stu-id="35713-121">Relationship</span></span> | <span data-ttu-id="35713-122">类型</span><span class="sxs-lookup"><span data-stu-id="35713-122">Type</span></span>        | <span data-ttu-id="35713-123">说明</span><span class="sxs-lookup"><span data-stu-id="35713-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="35713-124">id</span><span class="sxs-lookup"><span data-stu-id="35713-124">id</span></span> |<span data-ttu-id="35713-125">String</span><span class="sxs-lookup"><span data-stu-id="35713-125">String</span></span>| <span data-ttu-id="35713-126">组织的设置对象的 Id。</span><span class="sxs-lookup"><span data-stu-id="35713-126">Id of the settings object for the organization.</span></span> |
|<span data-ttu-id="35713-127">profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="35713-127">profileCardProperties</span></span>|<span data-ttu-id="35713-128">[profileCardProperty](profilecardproperty.md)集合</span><span class="sxs-lookup"><span data-stu-id="35713-128">[profileCardProperty](profilecardproperty.md) collection</span></span>| <span data-ttu-id="35713-129">包含管理员已定义为在 M365 配置文件卡上可见的属性的集合。</span><span class="sxs-lookup"><span data-stu-id="35713-129">Contains a collection of the properties an administrator has defined as visible on the M365 Profile Card.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="35713-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35713-130">JSON representation</span></span>

<span data-ttu-id="35713-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35713-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationSettings",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "profileCardProperties": [{"@odata.type": "microsoft.graph.profileCardProperty"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
