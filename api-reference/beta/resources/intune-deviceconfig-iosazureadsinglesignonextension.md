---
title: iosAzureAdSingleSignOnExtension 资源类型
description: 表示 iOS 设备的 Azure AD 类型单一登录扩展配置文件。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c9388b46457df2390a0820c1005f0df0e1cae9b2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444204"
---
# <a name="iosazureadsinglesignonextension-resource-type"></a><span data-ttu-id="d7b4e-103">iosAzureAdSingleSignOnExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7b4e-103">iosAzureAdSingleSignOnExtension resource type</span></span>

<span data-ttu-id="d7b4e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7b4e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7b4e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d7b4e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7b4e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d7b4e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7b4e-107">表示 iOS 设备的 Azure AD 类型单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="d7b4e-107">Represents an Azure AD-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="d7b4e-108">继承自[iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="d7b4e-108">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d7b4e-109">属性</span><span class="sxs-lookup"><span data-stu-id="d7b4e-109">Properties</span></span>
|<span data-ttu-id="d7b4e-110">属性</span><span class="sxs-lookup"><span data-stu-id="d7b4e-110">Property</span></span>|<span data-ttu-id="d7b4e-111">类型</span><span class="sxs-lookup"><span data-stu-id="d7b4e-111">Type</span></span>|<span data-ttu-id="d7b4e-112">说明</span><span class="sxs-lookup"><span data-stu-id="d7b4e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7b4e-113">enableSharedDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d7b4e-113">enableSharedDeviceMode</span></span>|<span data-ttu-id="d7b4e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7b4e-114">Boolean</span></span>|<span data-ttu-id="d7b4e-115">启用或禁用共享设备模式。</span><span class="sxs-lookup"><span data-stu-id="d7b4e-115">Enables or disables shared device mode.</span></span>|
|<span data-ttu-id="d7b4e-116">配置</span><span class="sxs-lookup"><span data-stu-id="d7b4e-116">configurations</span></span>|<span data-ttu-id="d7b4e-117">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)集合</span><span class="sxs-lookup"><span data-stu-id="d7b4e-117">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="d7b4e-118">获取或设置用于配置凭据类型配置文件的类型键/值对的列表。</span><span class="sxs-lookup"><span data-stu-id="d7b4e-118">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="d7b4e-119">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d7b4e-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7b4e-120">关系</span><span class="sxs-lookup"><span data-stu-id="d7b4e-120">Relationships</span></span>
<span data-ttu-id="d7b4e-121">无</span><span class="sxs-lookup"><span data-stu-id="d7b4e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7b4e-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7b4e-122">JSON Representation</span></span>
<span data-ttu-id="d7b4e-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7b4e-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAzureAdSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAzureAdSingleSignOnExtension",
  "enableSharedDeviceMode": true,
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyTypedValuePair",
      "key": "String"
    }
  ]
}
```



