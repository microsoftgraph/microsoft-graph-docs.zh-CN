---
title: omaSetting 资源类型
description: OMA 设置定义。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cffa929a063c77010f005a4e0b3da8fd8b7363d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530603"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="3a87f-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a87f-103">omaSetting resource type</span></span>

<span data-ttu-id="3a87f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a87f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a87f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3a87f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a87f-106">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="3a87f-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="3a87f-107">属性</span><span class="sxs-lookup"><span data-stu-id="3a87f-107">Properties</span></span>
|<span data-ttu-id="3a87f-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a87f-108">Property</span></span>|<span data-ttu-id="3a87f-109">类型</span><span class="sxs-lookup"><span data-stu-id="3a87f-109">Type</span></span>|<span data-ttu-id="3a87f-110">说明</span><span class="sxs-lookup"><span data-stu-id="3a87f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a87f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3a87f-111">displayName</span></span>|<span data-ttu-id="3a87f-112">字符串</span><span class="sxs-lookup"><span data-stu-id="3a87f-112">String</span></span>|<span data-ttu-id="3a87f-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="3a87f-113">Display Name.</span></span>|
|<span data-ttu-id="3a87f-114">说明</span><span class="sxs-lookup"><span data-stu-id="3a87f-114">description</span></span>|<span data-ttu-id="3a87f-115">字符串</span><span class="sxs-lookup"><span data-stu-id="3a87f-115">String</span></span>|<span data-ttu-id="3a87f-116">说明。</span><span class="sxs-lookup"><span data-stu-id="3a87f-116">Description.</span></span>|
|<span data-ttu-id="3a87f-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="3a87f-117">omaUri</span></span>|<span data-ttu-id="3a87f-118">String</span><span class="sxs-lookup"><span data-stu-id="3a87f-118">String</span></span>|<span data-ttu-id="3a87f-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="3a87f-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a87f-120">关系</span><span class="sxs-lookup"><span data-stu-id="3a87f-120">Relationships</span></span>
<span data-ttu-id="3a87f-121">无</span><span class="sxs-lookup"><span data-stu-id="3a87f-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a87f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a87f-122">JSON Representation</span></span>
<span data-ttu-id="3a87f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a87f-123">Here is a JSON representation of the resource.</span></span>
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




