---
title: iosAzureAdSingleSignOnExtension 资源类型
description: 表示 iOS 设备的 Azure AD 类型单一登录扩展配置文件。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cd1eacccc09926c65a8e5faf3c61321b472d2013
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790460"
---
# <a name="iosazureadsinglesignonextension-resource-type"></a><span data-ttu-id="8fe93-103">iosAzureAdSingleSignOnExtension 资源类型</span><span class="sxs-lookup"><span data-stu-id="8fe93-103">iosAzureAdSingleSignOnExtension resource type</span></span>

<span data-ttu-id="8fe93-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8fe93-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8fe93-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8fe93-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fe93-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8fe93-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fe93-107">表示 iOS 设备的 Azure AD 类型单一登录扩展配置文件。</span><span class="sxs-lookup"><span data-stu-id="8fe93-107">Represents an Azure AD-type Single Sign-On extension profile for iOS devices.</span></span>


<span data-ttu-id="8fe93-108">继承自 [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span><span class="sxs-lookup"><span data-stu-id="8fe93-108">Inherits from [iosSingleSignOnExtension](../resources/intune-deviceconfig-iossinglesignonextension.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8fe93-109">属性</span><span class="sxs-lookup"><span data-stu-id="8fe93-109">Properties</span></span>
|<span data-ttu-id="8fe93-110">属性</span><span class="sxs-lookup"><span data-stu-id="8fe93-110">Property</span></span>|<span data-ttu-id="8fe93-111">类型</span><span class="sxs-lookup"><span data-stu-id="8fe93-111">Type</span></span>|<span data-ttu-id="8fe93-112">说明</span><span class="sxs-lookup"><span data-stu-id="8fe93-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fe93-113">enableSharedDeviceMode</span><span class="sxs-lookup"><span data-stu-id="8fe93-113">enableSharedDeviceMode</span></span>|<span data-ttu-id="8fe93-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="8fe93-114">Boolean</span></span>|<span data-ttu-id="8fe93-115">启用或禁用共享设备模式。</span><span class="sxs-lookup"><span data-stu-id="8fe93-115">Enables or disables shared device mode.</span></span>|
|<span data-ttu-id="8fe93-116">bundleIdAccessControlList</span><span class="sxs-lookup"><span data-stu-id="8fe93-116">bundleIdAccessControlList</span></span>|<span data-ttu-id="8fe93-117">字符串集合</span><span class="sxs-lookup"><span data-stu-id="8fe93-117">String collection</span></span>|<span data-ttu-id="8fe93-118">允许为单一登录使用 AAD 扩展的附加捆绑捆绑 Id 的可选列表。</span><span class="sxs-lookup"><span data-stu-id="8fe93-118">An optional list of additional bundle IDs allowed to use the AAD extension for single sign-on.</span></span>|
|<span data-ttu-id="8fe93-119">配置</span><span class="sxs-lookup"><span data-stu-id="8fe93-119">configurations</span></span>|<span data-ttu-id="8fe93-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8fe93-120">[keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md) collection</span></span>|<span data-ttu-id="8fe93-121">获取或设置用于配置凭据类型配置文件的类型键/值对的列表。</span><span class="sxs-lookup"><span data-stu-id="8fe93-121">Gets or sets a list of typed key-value pairs used to configure Credential-type profiles.</span></span> <span data-ttu-id="8fe93-122">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8fe93-122">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8fe93-123">关系</span><span class="sxs-lookup"><span data-stu-id="8fe93-123">Relationships</span></span>
<span data-ttu-id="8fe93-124">无</span><span class="sxs-lookup"><span data-stu-id="8fe93-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8fe93-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8fe93-125">JSON Representation</span></span>
<span data-ttu-id="8fe93-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fe93-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAzureAdSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAzureAdSingleSignOnExtension",
  "enableSharedDeviceMode": true,
  "bundleIdAccessControlList": [
    "String"
  ],
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyTypedValuePair",
      "key": "String"
    }
  ]
}
```



