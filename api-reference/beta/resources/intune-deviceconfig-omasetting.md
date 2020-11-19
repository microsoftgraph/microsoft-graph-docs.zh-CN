---
title: omaSetting 资源类型
description: OMA 设置定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 59a0d38eca6e448457d208eb9981c9de51031489
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273184"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="a35fc-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="a35fc-103">omaSetting resource type</span></span>

<span data-ttu-id="a35fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a35fc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a35fc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a35fc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a35fc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a35fc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a35fc-107">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="a35fc-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="a35fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="a35fc-108">Properties</span></span>
|<span data-ttu-id="a35fc-109">属性</span><span class="sxs-lookup"><span data-stu-id="a35fc-109">Property</span></span>|<span data-ttu-id="a35fc-110">类型</span><span class="sxs-lookup"><span data-stu-id="a35fc-110">Type</span></span>|<span data-ttu-id="a35fc-111">说明</span><span class="sxs-lookup"><span data-stu-id="a35fc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a35fc-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a35fc-112">displayName</span></span>|<span data-ttu-id="a35fc-113">字符串</span><span class="sxs-lookup"><span data-stu-id="a35fc-113">String</span></span>|<span data-ttu-id="a35fc-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="a35fc-114">Display Name.</span></span>|
|<span data-ttu-id="a35fc-115">description</span><span class="sxs-lookup"><span data-stu-id="a35fc-115">description</span></span>|<span data-ttu-id="a35fc-116">字符串</span><span class="sxs-lookup"><span data-stu-id="a35fc-116">String</span></span>|<span data-ttu-id="a35fc-117">说明。</span><span class="sxs-lookup"><span data-stu-id="a35fc-117">Description.</span></span>|
|<span data-ttu-id="a35fc-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="a35fc-118">omaUri</span></span>|<span data-ttu-id="a35fc-119">String</span><span class="sxs-lookup"><span data-stu-id="a35fc-119">String</span></span>|<span data-ttu-id="a35fc-120">OMA。</span><span class="sxs-lookup"><span data-stu-id="a35fc-120">OMA.</span></span>|
|<span data-ttu-id="a35fc-121">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="a35fc-121">isEncrypted</span></span>|<span data-ttu-id="a35fc-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="a35fc-122">Boolean</span></span>|<span data-ttu-id="a35fc-123">指示是否对值字段进行加密。</span><span class="sxs-lookup"><span data-stu-id="a35fc-123">Indicates whether the value field is encrypted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a35fc-124">关系</span><span class="sxs-lookup"><span data-stu-id="a35fc-124">Relationships</span></span>
<span data-ttu-id="a35fc-125">无</span><span class="sxs-lookup"><span data-stu-id="a35fc-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a35fc-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a35fc-126">JSON Representation</span></span>
<span data-ttu-id="a35fc-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a35fc-127">Here is a JSON representation of the resource.</span></span>
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
  "omaUri": "String",
  "isEncrypted": true
}
```




