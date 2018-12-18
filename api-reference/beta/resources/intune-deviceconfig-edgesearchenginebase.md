---
title: edgeSearchEngineBase 资源类型
description: 允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。 如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。
author: tfitzmac
ms.openlocfilehash: c60dd1786f5a211947c02f1a9f5f048737ba3788
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346499"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="28d58-104">edgeSearchEngineBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="28d58-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="28d58-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="28d58-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28d58-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="28d58-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28d58-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="28d58-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28d58-108">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="28d58-108">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="28d58-109">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="28d58-109">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="28d58-110">属性</span><span class="sxs-lookup"><span data-stu-id="28d58-110">Properties</span></span>
|<span data-ttu-id="28d58-111">属性</span><span class="sxs-lookup"><span data-stu-id="28d58-111">Property</span></span>|<span data-ttu-id="28d58-112">类型</span><span class="sxs-lookup"><span data-stu-id="28d58-112">Type</span></span>|<span data-ttu-id="28d58-113">说明</span><span class="sxs-lookup"><span data-stu-id="28d58-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="28d58-114">关系</span><span class="sxs-lookup"><span data-stu-id="28d58-114">Relationships</span></span>
<span data-ttu-id="28d58-115">无</span><span class="sxs-lookup"><span data-stu-id="28d58-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="28d58-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28d58-116">JSON Representation</span></span>
<span data-ttu-id="28d58-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28d58-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineBase"
}
```





