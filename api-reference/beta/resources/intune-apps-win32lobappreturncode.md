---
title: win32LobAppReturnCode 资源类型
description: Win32 应用程序包含返回代码属性
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f635c49ece6a1083ef3a89271faf76e01206e9ed
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849817"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="dadfd-103">win32LobAppReturnCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="dadfd-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="dadfd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="dadfd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dadfd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="dadfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dadfd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dadfd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dadfd-107">Win32 应用程序包含返回代码属性</span><span class="sxs-lookup"><span data-stu-id="dadfd-107">Contains return code properties for a Win32 App</span></span>
## <a name="properties"></a><span data-ttu-id="dadfd-108">属性</span><span class="sxs-lookup"><span data-stu-id="dadfd-108">Properties</span></span>
|<span data-ttu-id="dadfd-109">属性</span><span class="sxs-lookup"><span data-stu-id="dadfd-109">Property</span></span>|<span data-ttu-id="dadfd-110">类型</span><span class="sxs-lookup"><span data-stu-id="dadfd-110">Type</span></span>|<span data-ttu-id="dadfd-111">Description</span><span class="sxs-lookup"><span data-stu-id="dadfd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dadfd-112">returnCode</span><span class="sxs-lookup"><span data-stu-id="dadfd-112">returnCode</span></span>|<span data-ttu-id="dadfd-113">Int32</span><span class="sxs-lookup"><span data-stu-id="dadfd-113">Int32</span></span>|<span data-ttu-id="dadfd-114">返回代码。</span><span class="sxs-lookup"><span data-stu-id="dadfd-114">Return code.</span></span>|
|<span data-ttu-id="dadfd-115">type</span><span class="sxs-lookup"><span data-stu-id="dadfd-115">type</span></span>|[<span data-ttu-id="dadfd-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="dadfd-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="dadfd-117">返回代码的类型。</span><span class="sxs-lookup"><span data-stu-id="dadfd-117">The type of return code.</span></span> <span data-ttu-id="dadfd-118">可取值为：`failed`、`success`、`softReboot`、`hardReboot`、`retry`。</span><span class="sxs-lookup"><span data-stu-id="dadfd-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dadfd-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="dadfd-119">Relationships</span></span>
<span data-ttu-id="dadfd-120">无</span><span class="sxs-lookup"><span data-stu-id="dadfd-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dadfd-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dadfd-121">JSON Representation</span></span>
<span data-ttu-id="dadfd-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dadfd-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```





