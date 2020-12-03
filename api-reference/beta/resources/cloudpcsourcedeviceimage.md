---
title: cloudPcSourceDeviceImage 资源类型
description: '与你的 Azure 订阅关联的源映像。 '
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c944ab1a634d10e978c6ce1620ebe1accc5e4359
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563742"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a><span data-ttu-id="edc6f-103">cloudPcSourceDeviceImage 资源类型</span><span class="sxs-lookup"><span data-stu-id="edc6f-103">cloudPcSourceDeviceImage resource type</span></span>

<span data-ttu-id="edc6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="edc6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="edc6f-105">与你的 Azure 订阅关联的源映像。</span><span class="sxs-lookup"><span data-stu-id="edc6f-105">The source image associated with your Azure subscription.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="edc6f-106">属性</span><span class="sxs-lookup"><span data-stu-id="edc6f-106">Properties</span></span>

|<span data-ttu-id="edc6f-107">属性</span><span class="sxs-lookup"><span data-stu-id="edc6f-107">Property</span></span>|<span data-ttu-id="edc6f-108">类型</span><span class="sxs-lookup"><span data-stu-id="edc6f-108">Type</span></span>|<span data-ttu-id="edc6f-109">说明</span><span class="sxs-lookup"><span data-stu-id="edc6f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="edc6f-110">id</span><span class="sxs-lookup"><span data-stu-id="edc6f-110">id</span></span>|<span data-ttu-id="edc6f-111">String</span><span class="sxs-lookup"><span data-stu-id="edc6f-111">String</span></span>|<span data-ttu-id="edc6f-112">源图像的 ID。</span><span class="sxs-lookup"><span data-stu-id="edc6f-112">The ID of the source image.</span></span>|
|<span data-ttu-id="edc6f-113">displayName</span><span class="sxs-lookup"><span data-stu-id="edc6f-113">displayName</span></span>|<span data-ttu-id="edc6f-114">String</span><span class="sxs-lookup"><span data-stu-id="edc6f-114">String</span></span>|<span data-ttu-id="edc6f-115">源图像的显示名称。</span><span class="sxs-lookup"><span data-stu-id="edc6f-115">The display name for the source image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="edc6f-116">关系</span><span class="sxs-lookup"><span data-stu-id="edc6f-116">Relationships</span></span>

<span data-ttu-id="edc6f-117">无。</span><span class="sxs-lookup"><span data-stu-id="edc6f-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="edc6f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="edc6f-118">JSON representation</span></span>

<span data-ttu-id="edc6f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="edc6f-119">The following is a JSON representation of the resource.</span></span>
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
