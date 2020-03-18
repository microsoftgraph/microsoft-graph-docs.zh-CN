---
title: resourceAction 资源类型
description: 资源的允许和不允许的操作的集合。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 48d687fd6878256c43e9c95e167432d3e7454695
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773733"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="3f75a-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f75a-103">resourceAction resource type</span></span>

> <span data-ttu-id="3f75a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3f75a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f75a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3f75a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f75a-106">资源的允许和不允许的操作的集合。</span><span class="sxs-lookup"><span data-stu-id="3f75a-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="3f75a-107">属性</span><span class="sxs-lookup"><span data-stu-id="3f75a-107">Properties</span></span>
|<span data-ttu-id="3f75a-108">属性</span><span class="sxs-lookup"><span data-stu-id="3f75a-108">Property</span></span>|<span data-ttu-id="3f75a-109">类型</span><span class="sxs-lookup"><span data-stu-id="3f75a-109">Type</span></span>|<span data-ttu-id="3f75a-110">说明</span><span class="sxs-lookup"><span data-stu-id="3f75a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f75a-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="3f75a-111">allowedResourceActions</span></span>|<span data-ttu-id="3f75a-112">字符串集合</span><span class="sxs-lookup"><span data-stu-id="3f75a-112">String collection</span></span>|<span data-ttu-id="3f75a-113">允许的操作</span><span class="sxs-lookup"><span data-stu-id="3f75a-113">Allowed Actions</span></span>|
|<span data-ttu-id="3f75a-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="3f75a-114">notAllowedResourceActions</span></span>|<span data-ttu-id="3f75a-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="3f75a-115">String collection</span></span>|<span data-ttu-id="3f75a-116">不允许操作。</span><span class="sxs-lookup"><span data-stu-id="3f75a-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f75a-117">关系</span><span class="sxs-lookup"><span data-stu-id="3f75a-117">Relationships</span></span>
<span data-ttu-id="3f75a-118">无</span><span class="sxs-lookup"><span data-stu-id="3f75a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f75a-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f75a-119">JSON Representation</span></span>
<span data-ttu-id="3f75a-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f75a-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



