---
title: iosHomeScreenItem 资源类型
description: 表示 iOS 主屏幕上的项
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ff573a6f7ae0d78113a32514bc312c3920b216f1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987620"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="34470-103">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="34470-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="34470-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="34470-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34470-105">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="34470-105">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="34470-106">属性</span><span class="sxs-lookup"><span data-stu-id="34470-106">Properties</span></span>
|<span data-ttu-id="34470-107">属性</span><span class="sxs-lookup"><span data-stu-id="34470-107">Property</span></span>|<span data-ttu-id="34470-108">类型</span><span class="sxs-lookup"><span data-stu-id="34470-108">Type</span></span>|<span data-ttu-id="34470-109">说明</span><span class="sxs-lookup"><span data-stu-id="34470-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34470-110">displayName</span><span class="sxs-lookup"><span data-stu-id="34470-110">displayName</span></span>|<span data-ttu-id="34470-111">String</span><span class="sxs-lookup"><span data-stu-id="34470-111">String</span></span>|<span data-ttu-id="34470-112">应用的名称</span><span class="sxs-lookup"><span data-stu-id="34470-112">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="34470-113">关系</span><span class="sxs-lookup"><span data-stu-id="34470-113">Relationships</span></span>
<span data-ttu-id="34470-114">无</span><span class="sxs-lookup"><span data-stu-id="34470-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="34470-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34470-115">JSON Representation</span></span>
<span data-ttu-id="34470-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34470-116">Here is a JSON representation of the resource.</span></span>
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



