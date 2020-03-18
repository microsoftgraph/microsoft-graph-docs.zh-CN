---
title: roleScopeTagInfo 资源类型
description: 包含 Role Scope Tag 对象的属性的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c932a1353f684771a1979ae970141d674f726142
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797407"
---
# <a name="rolescopetaginfo-resource-type"></a><span data-ttu-id="80f94-103">roleScopeTagInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="80f94-103">roleScopeTagInfo resource type</span></span>

> <span data-ttu-id="80f94-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="80f94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80f94-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="80f94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80f94-106">包含 Role Scope Tag 对象的属性的类。</span><span class="sxs-lookup"><span data-stu-id="80f94-106">A class containing the properties of Role Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="80f94-107">属性</span><span class="sxs-lookup"><span data-stu-id="80f94-107">Properties</span></span>
|<span data-ttu-id="80f94-108">属性</span><span class="sxs-lookup"><span data-stu-id="80f94-108">Property</span></span>|<span data-ttu-id="80f94-109">类型</span><span class="sxs-lookup"><span data-stu-id="80f94-109">Type</span></span>|<span data-ttu-id="80f94-110">说明</span><span class="sxs-lookup"><span data-stu-id="80f94-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80f94-111">displayName</span><span class="sxs-lookup"><span data-stu-id="80f94-111">displayName</span></span>|<span data-ttu-id="80f94-112">String</span><span class="sxs-lookup"><span data-stu-id="80f94-112">String</span></span>|<span data-ttu-id="80f94-113">范围标记显示名称。</span><span class="sxs-lookup"><span data-stu-id="80f94-113">Scope Tag Display name.</span></span>|
|<span data-ttu-id="80f94-114">roleScopeTagId</span><span class="sxs-lookup"><span data-stu-id="80f94-114">roleScopeTagId</span></span>|<span data-ttu-id="80f94-115">String</span><span class="sxs-lookup"><span data-stu-id="80f94-115">String</span></span>|<span data-ttu-id="80f94-116">范围标记 Id。</span><span class="sxs-lookup"><span data-stu-id="80f94-116">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80f94-117">关系</span><span class="sxs-lookup"><span data-stu-id="80f94-117">Relationships</span></span>
<span data-ttu-id="80f94-118">无</span><span class="sxs-lookup"><span data-stu-id="80f94-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80f94-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80f94-119">JSON Representation</span></span>
<span data-ttu-id="80f94-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80f94-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.roleScopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagInfo",
  "displayName": "String",
  "roleScopeTagId": "String"
}
```



