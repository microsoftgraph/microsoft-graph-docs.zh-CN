---
title: win32LobAppReturnCode 资源类型
description: 包含 Win32 应用的返回代码属性
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5e1c312fd7a43c6f685d80211849e9a9280917b8
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797547"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="d7d19-103">win32LobAppReturnCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7d19-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="d7d19-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d7d19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7d19-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d7d19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7d19-106">包含 Win32 应用的返回代码属性</span><span class="sxs-lookup"><span data-stu-id="d7d19-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="d7d19-107">属性</span><span class="sxs-lookup"><span data-stu-id="d7d19-107">Properties</span></span>
|<span data-ttu-id="d7d19-108">属性</span><span class="sxs-lookup"><span data-stu-id="d7d19-108">Property</span></span>|<span data-ttu-id="d7d19-109">类型</span><span class="sxs-lookup"><span data-stu-id="d7d19-109">Type</span></span>|<span data-ttu-id="d7d19-110">说明</span><span class="sxs-lookup"><span data-stu-id="d7d19-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7d19-111">returnCode</span><span class="sxs-lookup"><span data-stu-id="d7d19-111">returnCode</span></span>|<span data-ttu-id="d7d19-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d7d19-112">Int32</span></span>|<span data-ttu-id="d7d19-113">返回代码。</span><span class="sxs-lookup"><span data-stu-id="d7d19-113">Return code.</span></span>|
|<span data-ttu-id="d7d19-114">type</span><span class="sxs-lookup"><span data-stu-id="d7d19-114">type</span></span>|[<span data-ttu-id="d7d19-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="d7d19-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="d7d19-116">返回代码的类型。</span><span class="sxs-lookup"><span data-stu-id="d7d19-116">The type of return code.</span></span> <span data-ttu-id="d7d19-117">可取值为：`failed`、`success`、`softReboot`、`hardReboot`、`retry`。</span><span class="sxs-lookup"><span data-stu-id="d7d19-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7d19-118">关系</span><span class="sxs-lookup"><span data-stu-id="d7d19-118">Relationships</span></span>
<span data-ttu-id="d7d19-119">无</span><span class="sxs-lookup"><span data-stu-id="d7d19-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7d19-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7d19-120">JSON Representation</span></span>
<span data-ttu-id="d7d19-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7d19-121">Here is a JSON representation of the resource.</span></span>
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



