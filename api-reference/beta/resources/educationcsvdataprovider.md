---
title: educationCsvDataProvider 资源类型
description: '用于输入的源 CSV 文件时设置学校数据同步配置文件。  '
ms.openlocfilehash: a3079b4f18c74c95fb0f8646116f2c7901d17b3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041862"
---
# <a name="educationcsvdataprovider-resource-type"></a><span data-ttu-id="b45cd-103">educationCsvDataProvider 资源类型</span><span class="sxs-lookup"><span data-stu-id="b45cd-103">educationCsvDataProvider resource type</span></span>

> <span data-ttu-id="b45cd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b45cd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b45cd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b45cd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b45cd-106">用于输入的源 CSV 文件时设置学校数据同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="b45cd-106">Used to set up the school data synchronization profile when CSV files are the input source.</span></span>  

<span data-ttu-id="b45cd-107">派生自[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="b45cd-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b45cd-108">属性</span><span class="sxs-lookup"><span data-stu-id="b45cd-108">Properties</span></span>

| <span data-ttu-id="b45cd-109">属性</span><span class="sxs-lookup"><span data-stu-id="b45cd-109">Property</span></span> | <span data-ttu-id="b45cd-110">类型</span><span class="sxs-lookup"><span data-stu-id="b45cd-110">Type</span></span> | <span data-ttu-id="b45cd-111">说明</span><span class="sxs-lookup"><span data-stu-id="b45cd-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b45cd-112">**自定义项**</span><span class="sxs-lookup"><span data-stu-id="b45cd-112">**customizations**</span></span> | [<span data-ttu-id="b45cd-113">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="b45cd-113">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="b45cd-114">可选自定义项应用于同步配置文件。</span><span class="sxs-lookup"><span data-stu-id="b45cd-114">Optional customizations to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b45cd-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b45cd-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationCsvDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationCsvDataProvider",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
