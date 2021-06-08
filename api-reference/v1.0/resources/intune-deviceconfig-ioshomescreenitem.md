---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cf6f4aadbe49579ff556de791d7afe58ad1728c8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760055"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="6e948-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e948-103">iosHomeScreenItem resource type</span></span>

<span data-ttu-id="6e948-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e948-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e948-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e948-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e948-106">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="6e948-106">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="6e948-107">属性</span><span class="sxs-lookup"><span data-stu-id="6e948-107">Properties</span></span>
|<span data-ttu-id="6e948-108">属性</span><span class="sxs-lookup"><span data-stu-id="6e948-108">Property</span></span>|<span data-ttu-id="6e948-109">类型</span><span class="sxs-lookup"><span data-stu-id="6e948-109">Type</span></span>|<span data-ttu-id="6e948-110">说明</span><span class="sxs-lookup"><span data-stu-id="6e948-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e948-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6e948-111">displayName</span></span>|<span data-ttu-id="6e948-112">String</span><span class="sxs-lookup"><span data-stu-id="6e948-112">String</span></span>|<span data-ttu-id="6e948-113">应用的名称</span><span class="sxs-lookup"><span data-stu-id="6e948-113">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e948-114">关系</span><span class="sxs-lookup"><span data-stu-id="6e948-114">Relationships</span></span>
<span data-ttu-id="6e948-115">无</span><span class="sxs-lookup"><span data-stu-id="6e948-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e948-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e948-116">JSON Representation</span></span>
<span data-ttu-id="6e948-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e948-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```




