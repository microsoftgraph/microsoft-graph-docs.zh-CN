---
title: windows10AssociatedApps 资源类型
description: Windows 10 相关应用程序定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d1f6363027ae46263146efdbf3f5ac5254afcd93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911908"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="e189d-103">windows10AssociatedApps 资源类型</span><span class="sxs-lookup"><span data-stu-id="e189d-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="e189d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e189d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e189d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e189d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e189d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e189d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e189d-107">Windows 10 相关应用程序定义。</span><span class="sxs-lookup"><span data-stu-id="e189d-107">Windows 10 Associated Application definition.</span></span>
## <a name="properties"></a><span data-ttu-id="e189d-108">属性</span><span class="sxs-lookup"><span data-stu-id="e189d-108">Properties</span></span>
|<span data-ttu-id="e189d-109">属性</span><span class="sxs-lookup"><span data-stu-id="e189d-109">Property</span></span>|<span data-ttu-id="e189d-110">类型</span><span class="sxs-lookup"><span data-stu-id="e189d-110">Type</span></span>|<span data-ttu-id="e189d-111">Description</span><span class="sxs-lookup"><span data-stu-id="e189d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e189d-112">appType</span><span class="sxs-lookup"><span data-stu-id="e189d-112">appType</span></span>|[<span data-ttu-id="e189d-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="e189d-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="e189d-114">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="e189d-114">Application type.</span></span> <span data-ttu-id="e189d-115">可取值为：`desktop`、`universal`。</span><span class="sxs-lookup"><span data-stu-id="e189d-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="e189d-116">标识符</span><span class="sxs-lookup"><span data-stu-id="e189d-116">identifier</span></span>|<span data-ttu-id="e189d-117">字符串</span><span class="sxs-lookup"><span data-stu-id="e189d-117">String</span></span>|<span data-ttu-id="e189d-118">标识符。</span><span class="sxs-lookup"><span data-stu-id="e189d-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e189d-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="e189d-119">Relationships</span></span>
<span data-ttu-id="e189d-120">无</span><span class="sxs-lookup"><span data-stu-id="e189d-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e189d-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e189d-121">JSON Representation</span></span>
<span data-ttu-id="e189d-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e189d-122">Here is a JSON representation of the resource.</span></span>
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





