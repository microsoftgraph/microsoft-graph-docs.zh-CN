---
title: omaSetting 资源类型
description: OMA 设置定义。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6d0a69c10f1f0075caee48276bdbc37f6d616f22
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549550"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="193b6-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="193b6-103">omaSetting resource type</span></span>

> <span data-ttu-id="193b6-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="193b6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="193b6-105">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="193b6-105">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="193b6-106">属性</span><span class="sxs-lookup"><span data-stu-id="193b6-106">Properties</span></span>
|<span data-ttu-id="193b6-107">属性</span><span class="sxs-lookup"><span data-stu-id="193b6-107">Property</span></span>|<span data-ttu-id="193b6-108">类型</span><span class="sxs-lookup"><span data-stu-id="193b6-108">Type</span></span>|<span data-ttu-id="193b6-109">说明</span><span class="sxs-lookup"><span data-stu-id="193b6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="193b6-110">displayName</span><span class="sxs-lookup"><span data-stu-id="193b6-110">displayName</span></span>|<span data-ttu-id="193b6-111">字符串</span><span class="sxs-lookup"><span data-stu-id="193b6-111">String</span></span>|<span data-ttu-id="193b6-112">显示名称。</span><span class="sxs-lookup"><span data-stu-id="193b6-112">Display Name.</span></span>|
|<span data-ttu-id="193b6-113">description</span><span class="sxs-lookup"><span data-stu-id="193b6-113">description</span></span>|<span data-ttu-id="193b6-114">String</span><span class="sxs-lookup"><span data-stu-id="193b6-114">String</span></span>|<span data-ttu-id="193b6-115">说明。</span><span class="sxs-lookup"><span data-stu-id="193b6-115">Description.</span></span>|
|<span data-ttu-id="193b6-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="193b6-116">omaUri</span></span>|<span data-ttu-id="193b6-117">String</span><span class="sxs-lookup"><span data-stu-id="193b6-117">String</span></span>|<span data-ttu-id="193b6-118">OMA。</span><span class="sxs-lookup"><span data-stu-id="193b6-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="193b6-119">关系</span><span class="sxs-lookup"><span data-stu-id="193b6-119">Relationships</span></span>
<span data-ttu-id="193b6-120">无</span><span class="sxs-lookup"><span data-stu-id="193b6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="193b6-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="193b6-121">JSON Representation</span></span>
<span data-ttu-id="193b6-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="193b6-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



