---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
ms.openlocfilehash: 705849569dd91d339633e52187d16dfdd25b5ab3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046784"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="0037b-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="0037b-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="0037b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0037b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0037b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0037b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0037b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0037b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0037b-107">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="0037b-107">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="0037b-108">属性</span><span class="sxs-lookup"><span data-stu-id="0037b-108">Properties</span></span>
|<span data-ttu-id="0037b-109">属性</span><span class="sxs-lookup"><span data-stu-id="0037b-109">Property</span></span>|<span data-ttu-id="0037b-110">类型</span><span class="sxs-lookup"><span data-stu-id="0037b-110">Type</span></span>|<span data-ttu-id="0037b-111">说明</span><span class="sxs-lookup"><span data-stu-id="0037b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0037b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0037b-112">displayName</span></span>|<span data-ttu-id="0037b-113">String</span><span class="sxs-lookup"><span data-stu-id="0037b-113">String</span></span>|<span data-ttu-id="0037b-114">应用的名称</span><span class="sxs-lookup"><span data-stu-id="0037b-114">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="0037b-115">关系</span><span class="sxs-lookup"><span data-stu-id="0037b-115">Relationships</span></span>
<span data-ttu-id="0037b-116">无</span><span class="sxs-lookup"><span data-stu-id="0037b-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0037b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0037b-117">JSON Representation</span></span>
<span data-ttu-id="0037b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0037b-118">Here is a JSON representation of the resource.</span></span>
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





