---
title: windows10AssociatedApps 资源类型
description: Windows 10 相关应用程序定义。
author: tfitzmac
ms.openlocfilehash: a990d3b1f9b2b33a1e98fd30f5dea4da7fbf4ae8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344826"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="243d8-103">windows10AssociatedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="243d8-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="243d8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="243d8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="243d8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="243d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="243d8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="243d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="243d8-107">Windows 10 相关应用程序定义。</span><span class="sxs-lookup"><span data-stu-id="243d8-107">Windows 10 Associated Application definition.</span></span>
## <a name="properties"></a><span data-ttu-id="243d8-108">属性</span><span class="sxs-lookup"><span data-stu-id="243d8-108">Properties</span></span>
|<span data-ttu-id="243d8-109">属性</span><span class="sxs-lookup"><span data-stu-id="243d8-109">Property</span></span>|<span data-ttu-id="243d8-110">类型</span><span class="sxs-lookup"><span data-stu-id="243d8-110">Type</span></span>|<span data-ttu-id="243d8-111">说明</span><span class="sxs-lookup"><span data-stu-id="243d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="243d8-112">appType</span><span class="sxs-lookup"><span data-stu-id="243d8-112">appType</span></span>|[<span data-ttu-id="243d8-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="243d8-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="243d8-114">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="243d8-114">Application type.</span></span> <span data-ttu-id="243d8-115">可取值为：`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="243d8-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="243d8-116">标识符</span><span class="sxs-lookup"><span data-stu-id="243d8-116">identifier</span></span>|<span data-ttu-id="243d8-117">字符串</span><span class="sxs-lookup"><span data-stu-id="243d8-117">String</span></span>|<span data-ttu-id="243d8-118">标识符。</span><span class="sxs-lookup"><span data-stu-id="243d8-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="243d8-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="243d8-119">Relationships</span></span>
<span data-ttu-id="243d8-120">无</span><span class="sxs-lookup"><span data-stu-id="243d8-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="243d8-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="243d8-121">JSON Representation</span></span>
<span data-ttu-id="243d8-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="243d8-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```





