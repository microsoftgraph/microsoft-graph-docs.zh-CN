---
title: scopeTagInfo 资源类型
description: 包含 Scope 标记对象的属性的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c8238881d8a14cb8aa1dfcc01031105be0069c21
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538502"
---
# <a name="scopetaginfo-resource-type"></a><span data-ttu-id="a3b3a-103">scopeTagInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3b3a-103">scopeTagInfo resource type</span></span>

> <span data-ttu-id="a3b3a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3b3a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3b3a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3b3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3b3a-106">包含 Scope 标记对象的属性的类。</span><span class="sxs-lookup"><span data-stu-id="a3b3a-106">A class containing the properties of Scope Tag Object.</span></span>

## <a name="properties"></a><span data-ttu-id="a3b3a-107">属性</span><span class="sxs-lookup"><span data-stu-id="a3b3a-107">Properties</span></span>
|<span data-ttu-id="a3b3a-108">属性</span><span class="sxs-lookup"><span data-stu-id="a3b3a-108">Property</span></span>|<span data-ttu-id="a3b3a-109">类型</span><span class="sxs-lookup"><span data-stu-id="a3b3a-109">Type</span></span>|<span data-ttu-id="a3b3a-110">说明</span><span class="sxs-lookup"><span data-stu-id="a3b3a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3b3a-111">scopeTagName</span><span class="sxs-lookup"><span data-stu-id="a3b3a-111">scopeTagName</span></span>|<span data-ttu-id="a3b3a-112">字符串</span><span class="sxs-lookup"><span data-stu-id="a3b3a-112">String</span></span>|<span data-ttu-id="a3b3a-113">范围标记显示名称。</span><span class="sxs-lookup"><span data-stu-id="a3b3a-113">Scope Tag Display name.</span></span>|
|<span data-ttu-id="a3b3a-114">scopeTagId</span><span class="sxs-lookup"><span data-stu-id="a3b3a-114">scopeTagId</span></span>|<span data-ttu-id="a3b3a-115">字符串</span><span class="sxs-lookup"><span data-stu-id="a3b3a-115">String</span></span>|<span data-ttu-id="a3b3a-116">范围标记 Id。</span><span class="sxs-lookup"><span data-stu-id="a3b3a-116">Scope Tag Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3b3a-117">关系</span><span class="sxs-lookup"><span data-stu-id="a3b3a-117">Relationships</span></span>
<span data-ttu-id="a3b3a-118">无</span><span class="sxs-lookup"><span data-stu-id="a3b3a-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3b3a-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3b3a-119">JSON Representation</span></span>
<span data-ttu-id="a3b3a-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3b3a-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.scopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scopeTagInfo",
  "scopeTagName": "String",
  "scopeTagId": "String"
}
```



