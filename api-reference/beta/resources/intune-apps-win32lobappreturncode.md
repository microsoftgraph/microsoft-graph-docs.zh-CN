---
title: win32LobAppReturnCode 资源类型
description: 包含 Win32 应用的返回代码属性
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e7429433f4e1a382d0a5f4ba0dab6028bf27d283
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070973"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="167ee-103">win32LobAppReturnCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="167ee-103">win32LobAppReturnCode resource type</span></span>

<span data-ttu-id="167ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="167ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="167ee-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="167ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="167ee-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="167ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="167ee-107">包含 Win32 应用的返回代码属性</span><span class="sxs-lookup"><span data-stu-id="167ee-107">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="167ee-108">属性</span><span class="sxs-lookup"><span data-stu-id="167ee-108">Properties</span></span>
|<span data-ttu-id="167ee-109">属性</span><span class="sxs-lookup"><span data-stu-id="167ee-109">Property</span></span>|<span data-ttu-id="167ee-110">类型</span><span class="sxs-lookup"><span data-stu-id="167ee-110">Type</span></span>|<span data-ttu-id="167ee-111">说明</span><span class="sxs-lookup"><span data-stu-id="167ee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="167ee-112">returnCode</span><span class="sxs-lookup"><span data-stu-id="167ee-112">returnCode</span></span>|<span data-ttu-id="167ee-113">Int32</span><span class="sxs-lookup"><span data-stu-id="167ee-113">Int32</span></span>|<span data-ttu-id="167ee-114">返回代码。</span><span class="sxs-lookup"><span data-stu-id="167ee-114">Return code.</span></span>|
|<span data-ttu-id="167ee-115">type</span><span class="sxs-lookup"><span data-stu-id="167ee-115">type</span></span>|[<span data-ttu-id="167ee-116">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="167ee-116">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="167ee-117">返回代码的类型。</span><span class="sxs-lookup"><span data-stu-id="167ee-117">The type of return code.</span></span> <span data-ttu-id="167ee-118">可取值为：`failed`、`success`、`softReboot`、`hardReboot`、`retry`。</span><span class="sxs-lookup"><span data-stu-id="167ee-118">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="167ee-119">关系</span><span class="sxs-lookup"><span data-stu-id="167ee-119">Relationships</span></span>
<span data-ttu-id="167ee-120">无</span><span class="sxs-lookup"><span data-stu-id="167ee-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="167ee-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="167ee-121">JSON Representation</span></span>
<span data-ttu-id="167ee-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="167ee-122">Here is a JSON representation of the resource.</span></span>
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






