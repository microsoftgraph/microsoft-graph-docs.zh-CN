---
title: appConfigurationSettingItem 资源类型
description: 包含应用配置设置项的属性。
ms.openlocfilehash: bd08b325fd04e8e4a742da515d052d453cfb58a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009441"
---
# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="2b5cf-103">appConfigurationSettingItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b5cf-103">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="2b5cf-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2b5cf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b5cf-105">包含应用配置设置项的属性。</span><span class="sxs-lookup"><span data-stu-id="2b5cf-105">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="2b5cf-106">属性</span><span class="sxs-lookup"><span data-stu-id="2b5cf-106">Properties</span></span>
|<span data-ttu-id="2b5cf-107">属性</span><span class="sxs-lookup"><span data-stu-id="2b5cf-107">Property</span></span>|<span data-ttu-id="2b5cf-108">类型</span><span class="sxs-lookup"><span data-stu-id="2b5cf-108">Type</span></span>|<span data-ttu-id="2b5cf-109">说明</span><span class="sxs-lookup"><span data-stu-id="2b5cf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b5cf-110">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="2b5cf-110">appConfigKey</span></span>|<span data-ttu-id="2b5cf-111">String</span><span class="sxs-lookup"><span data-stu-id="2b5cf-111">String</span></span>|<span data-ttu-id="2b5cf-112">应用配置密钥。</span><span class="sxs-lookup"><span data-stu-id="2b5cf-112">app configuration key.</span></span>|
|<span data-ttu-id="2b5cf-113">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="2b5cf-113">appConfigKeyType</span></span>|[<span data-ttu-id="2b5cf-114">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="2b5cf-114">mdmAppConfigKeyType</span></span>](../resources/intune-apps-mdmappconfigkeytype.md)|<span data-ttu-id="2b5cf-115">应用配置密钥类型。</span><span class="sxs-lookup"><span data-stu-id="2b5cf-115">app configuration key type.</span></span> <span data-ttu-id="2b5cf-116">可取值为：`stringType`、`integerType`、`realType`、`booleanType`、`tokenType`。</span><span class="sxs-lookup"><span data-stu-id="2b5cf-116">Possible values are: `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`.</span></span>|
|<span data-ttu-id="2b5cf-117">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="2b5cf-117">appConfigKeyValue</span></span>|<span data-ttu-id="2b5cf-118">String</span><span class="sxs-lookup"><span data-stu-id="2b5cf-118">String</span></span>|<span data-ttu-id="2b5cf-119">应用配置密钥值。</span><span class="sxs-lookup"><span data-stu-id="2b5cf-119">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b5cf-120">关系</span><span class="sxs-lookup"><span data-stu-id="2b5cf-120">Relationships</span></span>
<span data-ttu-id="2b5cf-121">无</span><span class="sxs-lookup"><span data-stu-id="2b5cf-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2b5cf-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b5cf-122">JSON Representation</span></span>
<span data-ttu-id="2b5cf-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b5cf-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



