---
title: edgeHomeButtonOpensCustomURL 资源类型
description: 显示 "主页" 按钮;单击 "主页" 按钮，将加载特定的 URL。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fdf8771dec9bd27a74f3a3e0f60d2106733d5c8c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199145"
---
# <a name="edgehomebuttonopenscustomurl-resource-type"></a><span data-ttu-id="d6f4f-103">edgeHomeButtonOpensCustomURL 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6f4f-103">edgeHomeButtonOpensCustomURL resource type</span></span>

<span data-ttu-id="d6f4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6f4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6f4f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6f4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6f4f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6f4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6f4f-107">显示 "主页" 按钮;单击 "主页" 按钮，将加载特定的 URL。</span><span class="sxs-lookup"><span data-stu-id="d6f4f-107">Show the home button; clicking the home button loads a specific URL.</span></span>


<span data-ttu-id="d6f4f-108">继承自 [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6f4f-108">Inherits from [edgeHomeButtonConfiguration](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d6f4f-109">属性</span><span class="sxs-lookup"><span data-stu-id="d6f4f-109">Properties</span></span>
|<span data-ttu-id="d6f4f-110">属性</span><span class="sxs-lookup"><span data-stu-id="d6f4f-110">Property</span></span>|<span data-ttu-id="d6f4f-111">类型</span><span class="sxs-lookup"><span data-stu-id="d6f4f-111">Type</span></span>|<span data-ttu-id="d6f4f-112">说明</span><span class="sxs-lookup"><span data-stu-id="d6f4f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6f4f-113">homeButtonCustomURL</span><span class="sxs-lookup"><span data-stu-id="d6f4f-113">homeButtonCustomURL</span></span>|<span data-ttu-id="d6f4f-114">String</span><span class="sxs-lookup"><span data-stu-id="d6f4f-114">String</span></span>|<span data-ttu-id="d6f4f-115">要加载的特定 URL。</span><span class="sxs-lookup"><span data-stu-id="d6f4f-115">The specific URL to load.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6f4f-116">关系</span><span class="sxs-lookup"><span data-stu-id="d6f4f-116">Relationships</span></span>
<span data-ttu-id="d6f4f-117">无</span><span class="sxs-lookup"><span data-stu-id="d6f4f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6f4f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6f4f-118">JSON Representation</span></span>
<span data-ttu-id="d6f4f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6f4f-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeHomeButtonOpensCustomURL"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeHomeButtonOpensCustomURL",
  "homeButtonCustomURL": "String"
}
```




