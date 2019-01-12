---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 95dded55228cd6779de84db1bd8da1b745791c39
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948112"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="d9ceb-103">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9ceb-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="d9ceb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d9ceb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9ceb-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d9ceb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9ceb-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d9ceb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9ceb-107">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="d9ceb-107">BitLocker Removable Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="d9ceb-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9ceb-108">Properties</span></span>
|<span data-ttu-id="d9ceb-109">属性</span><span class="sxs-lookup"><span data-stu-id="d9ceb-109">Property</span></span>|<span data-ttu-id="d9ceb-110">类型</span><span class="sxs-lookup"><span data-stu-id="d9ceb-110">Type</span></span>|<span data-ttu-id="d9ceb-111">说明</span><span class="sxs-lookup"><span data-stu-id="d9ceb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9ceb-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="d9ceb-112">encryptionMethod</span></span>|[<span data-ttu-id="d9ceb-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="d9ceb-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="d9ceb-114">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="d9ceb-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="d9ceb-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="d9ceb-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="d9ceb-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="d9ceb-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="d9ceb-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9ceb-117">Boolean</span></span>|<span data-ttu-id="d9ceb-118">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="d9ceb-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="d9ceb-119">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="d9ceb-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="d9ceb-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="d9ceb-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="d9ceb-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9ceb-121">Boolean</span></span>|<span data-ttu-id="d9ceb-122">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="d9ceb-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9ceb-123">关系</span><span class="sxs-lookup"><span data-stu-id="d9ceb-123">Relationships</span></span>
<span data-ttu-id="d9ceb-124">无</span><span class="sxs-lookup"><span data-stu-id="d9ceb-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d9ceb-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9ceb-125">JSON Representation</span></span>
<span data-ttu-id="d9ceb-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9ceb-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```





