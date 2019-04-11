---
title: win32LobAppReturnCode 资源类型
description: 包含 Win32 应用的返回代码属性
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c05d695b05a001e6854e254bf065d6fb41ba773
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791346"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="b62bc-103">win32LobAppReturnCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="b62bc-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="b62bc-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b62bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b62bc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b62bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b62bc-106">包含 Win32 应用的返回代码属性</span><span class="sxs-lookup"><span data-stu-id="b62bc-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="b62bc-107">属性</span><span class="sxs-lookup"><span data-stu-id="b62bc-107">Properties</span></span>
|<span data-ttu-id="b62bc-108">属性</span><span class="sxs-lookup"><span data-stu-id="b62bc-108">Property</span></span>|<span data-ttu-id="b62bc-109">类型</span><span class="sxs-lookup"><span data-stu-id="b62bc-109">Type</span></span>|<span data-ttu-id="b62bc-110">说明</span><span class="sxs-lookup"><span data-stu-id="b62bc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b62bc-111">returnCode</span><span class="sxs-lookup"><span data-stu-id="b62bc-111">returnCode</span></span>|<span data-ttu-id="b62bc-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b62bc-112">Int32</span></span>|<span data-ttu-id="b62bc-113">返回代码。</span><span class="sxs-lookup"><span data-stu-id="b62bc-113">Return code.</span></span>|
|<span data-ttu-id="b62bc-114">类型</span><span class="sxs-lookup"><span data-stu-id="b62bc-114">type</span></span>|[<span data-ttu-id="b62bc-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="b62bc-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="b62bc-116">返回代码的类型。</span><span class="sxs-lookup"><span data-stu-id="b62bc-116">The type of return code.</span></span> <span data-ttu-id="b62bc-117">可取值为：`failed`、`success`、`softReboot`、`hardReboot` 或 `retry`。</span><span class="sxs-lookup"><span data-stu-id="b62bc-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b62bc-118">关系</span><span class="sxs-lookup"><span data-stu-id="b62bc-118">Relationships</span></span>
<span data-ttu-id="b62bc-119">无</span><span class="sxs-lookup"><span data-stu-id="b62bc-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b62bc-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b62bc-120">JSON Representation</span></span>
<span data-ttu-id="b62bc-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b62bc-121">Here is a JSON representation of the resource.</span></span>
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





