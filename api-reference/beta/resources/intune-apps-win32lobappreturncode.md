---
title: win32LobAppReturnCode 资源类型
description: 包含 Win32 应用的返回代码属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84b2798956ec2b88b4c4dea212fb614f26ff1eff
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335485"
---
# <a name="win32lobappreturncode-resource-type"></a><span data-ttu-id="b21db-103">win32LobAppReturnCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="b21db-103">win32LobAppReturnCode resource type</span></span>

> <span data-ttu-id="b21db-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b21db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b21db-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b21db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b21db-106">包含 Win32 应用的返回代码属性</span><span class="sxs-lookup"><span data-stu-id="b21db-106">Contains return code properties for a Win32 App</span></span>

## <a name="properties"></a><span data-ttu-id="b21db-107">属性</span><span class="sxs-lookup"><span data-stu-id="b21db-107">Properties</span></span>
|<span data-ttu-id="b21db-108">属性</span><span class="sxs-lookup"><span data-stu-id="b21db-108">Property</span></span>|<span data-ttu-id="b21db-109">类型</span><span class="sxs-lookup"><span data-stu-id="b21db-109">Type</span></span>|<span data-ttu-id="b21db-110">说明</span><span class="sxs-lookup"><span data-stu-id="b21db-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b21db-111">returnCode</span><span class="sxs-lookup"><span data-stu-id="b21db-111">returnCode</span></span>|<span data-ttu-id="b21db-112">Int32</span><span class="sxs-lookup"><span data-stu-id="b21db-112">Int32</span></span>|<span data-ttu-id="b21db-113">返回代码。</span><span class="sxs-lookup"><span data-stu-id="b21db-113">Return code.</span></span>|
|<span data-ttu-id="b21db-114">type</span><span class="sxs-lookup"><span data-stu-id="b21db-114">type</span></span>|[<span data-ttu-id="b21db-115">win32LobAppReturnCodeType</span><span class="sxs-lookup"><span data-stu-id="b21db-115">win32LobAppReturnCodeType</span></span>](../resources/intune-apps-win32lobappreturncodetype.md)|<span data-ttu-id="b21db-116">返回代码的类型。</span><span class="sxs-lookup"><span data-stu-id="b21db-116">The type of return code.</span></span> <span data-ttu-id="b21db-117">可取值为：`failed`、`success`、`softReboot`、`hardReboot`、`retry`。</span><span class="sxs-lookup"><span data-stu-id="b21db-117">Possible values are: `failed`, `success`, `softReboot`, `hardReboot`, `retry`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b21db-118">关系</span><span class="sxs-lookup"><span data-stu-id="b21db-118">Relationships</span></span>
<span data-ttu-id="b21db-119">无</span><span class="sxs-lookup"><span data-stu-id="b21db-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b21db-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b21db-120">JSON Representation</span></span>
<span data-ttu-id="b21db-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b21db-121">Here is a JSON representation of the resource.</span></span>
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



