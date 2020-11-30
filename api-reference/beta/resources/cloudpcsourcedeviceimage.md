---
title: cloudPcSourceDeviceImage 资源类型
description: '与你的 Azure 订阅关联的源映像。 '
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: eddae0ed023fb60c290067f3520ef90a67dec23b
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378277"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a><span data-ttu-id="6b7af-103">cloudPcSourceDeviceImage 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b7af-103">cloudPcSourceDeviceImage resource type</span></span>

<span data-ttu-id="6b7af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b7af-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b7af-105">与你的 Azure 订阅关联的源映像。</span><span class="sxs-lookup"><span data-stu-id="6b7af-105">The source image associated with your Azure subscription.</span></span>

## <a name="properties"></a><span data-ttu-id="6b7af-106">属性</span><span class="sxs-lookup"><span data-stu-id="6b7af-106">Properties</span></span>

|<span data-ttu-id="6b7af-107">属性</span><span class="sxs-lookup"><span data-stu-id="6b7af-107">Property</span></span>|<span data-ttu-id="6b7af-108">类型</span><span class="sxs-lookup"><span data-stu-id="6b7af-108">Type</span></span>|<span data-ttu-id="6b7af-109">说明</span><span class="sxs-lookup"><span data-stu-id="6b7af-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b7af-110">id</span><span class="sxs-lookup"><span data-stu-id="6b7af-110">id</span></span>|<span data-ttu-id="6b7af-111">字符串</span><span class="sxs-lookup"><span data-stu-id="6b7af-111">String</span></span>|<span data-ttu-id="6b7af-112">源图像的 ID。</span><span class="sxs-lookup"><span data-stu-id="6b7af-112">The ID of the source image.</span></span>|
|<span data-ttu-id="6b7af-113">displayName</span><span class="sxs-lookup"><span data-stu-id="6b7af-113">displayName</span></span>|<span data-ttu-id="6b7af-114">字符串</span><span class="sxs-lookup"><span data-stu-id="6b7af-114">String</span></span>|<span data-ttu-id="6b7af-115">源图像的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6b7af-115">The display name for the source image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b7af-116">关系</span><span class="sxs-lookup"><span data-stu-id="6b7af-116">Relationships</span></span>

<span data-ttu-id="6b7af-117">无。</span><span class="sxs-lookup"><span data-stu-id="6b7af-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b7af-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b7af-118">JSON representation</span></span>

<span data-ttu-id="6b7af-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b7af-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage",
  "baseType": "microsoft.graph.entity"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String"
}
```
