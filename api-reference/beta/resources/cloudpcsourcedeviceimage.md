---
title: cloudPcSourceDeviceImage 资源类型
description: '与 Azure 订阅关联的源映像。 '
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 1b0c656142ddad5af3d0af7778d0ae04f0c5d7b4
ms.sourcegitcommit: de175a11806f9e9ba3c916384e897aee1cc7f75c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/09/2021
ms.locfileid: "49790739"
---
# <a name="cloudpcsourcedeviceimage-resource-type"></a><span data-ttu-id="0dc2a-103">cloudPcSourceDeviceImage 资源类型</span><span class="sxs-lookup"><span data-stu-id="0dc2a-103">cloudPcSourceDeviceImage resource type</span></span>

<span data-ttu-id="0dc2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dc2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dc2a-105">与 Azure 订阅关联的源映像。</span><span class="sxs-lookup"><span data-stu-id="0dc2a-105">The source image associated with your Azure subscription.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="0dc2a-106">属性</span><span class="sxs-lookup"><span data-stu-id="0dc2a-106">Properties</span></span>

|<span data-ttu-id="0dc2a-107">属性</span><span class="sxs-lookup"><span data-stu-id="0dc2a-107">Property</span></span>|<span data-ttu-id="0dc2a-108">类型</span><span class="sxs-lookup"><span data-stu-id="0dc2a-108">Type</span></span>|<span data-ttu-id="0dc2a-109">说明</span><span class="sxs-lookup"><span data-stu-id="0dc2a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dc2a-110">id</span><span class="sxs-lookup"><span data-stu-id="0dc2a-110">id</span></span>|<span data-ttu-id="0dc2a-111">String</span><span class="sxs-lookup"><span data-stu-id="0dc2a-111">String</span></span>|<span data-ttu-id="0dc2a-112">源映像的 ID。</span><span class="sxs-lookup"><span data-stu-id="0dc2a-112">The ID of the source image.</span></span>|
|<span data-ttu-id="0dc2a-113">displayName</span><span class="sxs-lookup"><span data-stu-id="0dc2a-113">displayName</span></span>|<span data-ttu-id="0dc2a-114">String</span><span class="sxs-lookup"><span data-stu-id="0dc2a-114">String</span></span>|<span data-ttu-id="0dc2a-115">源显示名称的源图像。</span><span class="sxs-lookup"><span data-stu-id="0dc2a-115">The display name for the source image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0dc2a-116">关系</span><span class="sxs-lookup"><span data-stu-id="0dc2a-116">Relationships</span></span>

<span data-ttu-id="0dc2a-117">无。</span><span class="sxs-lookup"><span data-stu-id="0dc2a-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0dc2a-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0dc2a-118">JSON representation</span></span>

<span data-ttu-id="0dc2a-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0dc2a-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcSourceDeviceImage"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcSourceDeviceImage",
  "id": "String (identifier)",
  "displayName": "String"
}
```
