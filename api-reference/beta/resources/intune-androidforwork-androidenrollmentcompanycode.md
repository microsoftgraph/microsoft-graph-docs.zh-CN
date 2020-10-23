---
title: androidEnrollmentCompanyCode 资源类型
description: 用于保存用于通过 Google 的 Android 管理 API （如令牌、Url 和 QR 代码内容）进行注册的专业注册数据的类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ffb11de69dfe1f2a6a82e59024518b4d68676844
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736336"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="f7ef8-103">androidEnrollmentCompanyCode 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7ef8-103">androidEnrollmentCompanyCode resource type</span></span>

<span data-ttu-id="f7ef8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7ef8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7ef8-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7ef8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7ef8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7ef8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7ef8-107">用于保存用于通过 Google 的 Android 管理 API （如令牌、Url 和 QR 代码内容）进行注册的专业注册数据的类</span><span class="sxs-lookup"><span data-stu-id="f7ef8-107">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="f7ef8-108">属性</span><span class="sxs-lookup"><span data-stu-id="f7ef8-108">Properties</span></span>
|<span data-ttu-id="f7ef8-109">属性</span><span class="sxs-lookup"><span data-stu-id="f7ef8-109">Property</span></span>|<span data-ttu-id="f7ef8-110">类型</span><span class="sxs-lookup"><span data-stu-id="f7ef8-110">Type</span></span>|<span data-ttu-id="f7ef8-111">说明</span><span class="sxs-lookup"><span data-stu-id="f7ef8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7ef8-112">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="f7ef8-112">enrollmentToken</span></span>|<span data-ttu-id="f7ef8-113">String</span><span class="sxs-lookup"><span data-stu-id="f7ef8-113">String</span></span>|<span data-ttu-id="f7ef8-114">用户用于注册其设备的注册令牌。</span><span class="sxs-lookup"><span data-stu-id="f7ef8-114">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="f7ef8-115">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="f7ef8-115">qrCodeContent</span></span>|<span data-ttu-id="f7ef8-116">String</span><span class="sxs-lookup"><span data-stu-id="f7ef8-116">String</span></span>|<span data-ttu-id="f7ef8-117">用于生成此令牌的 QR 码的字符串。</span><span class="sxs-lookup"><span data-stu-id="f7ef8-117">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="f7ef8-118">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="f7ef8-118">qrCodeImage</span></span>|[<span data-ttu-id="f7ef8-119">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f7ef8-119">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f7ef8-120">为令牌生成的 QR 代码。</span><span class="sxs-lookup"><span data-stu-id="f7ef8-120">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7ef8-121">关系</span><span class="sxs-lookup"><span data-stu-id="f7ef8-121">Relationships</span></span>
<span data-ttu-id="f7ef8-122">无</span><span class="sxs-lookup"><span data-stu-id="f7ef8-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7ef8-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7ef8-123">JSON Representation</span></span>
<span data-ttu-id="f7ef8-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7ef8-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```





