---
title: macOSPrivacyAccessControlItem 资源类型
description: 表示每个进程的隐私首选项。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 90e73831f6dd3b8163a1c0d9c11b7944c9623958
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59091711"
---
# <a name="macosprivacyaccesscontrolitem-resource-type"></a>macOSPrivacyAccessControlItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示每个进程的隐私首选项。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|应用显示名称或可执行文件的名称。|
|标识符|String|应用、进程或可执行文件的捆绑 ID 或路径。|
|identifierType|[macOSProcessIdentifierType](../resources/intune-deviceconfig-macosprocessidentifiertype.md)|捆绑包 ID 用于标识应用。 路径用于标识进程或可执行文件。 可取值为：`bundleID`、`path`。|
|codeRequirement|String|输入代码要求，可通过终端应用中的命令"codesign –display -r –"获取。 在"=>"之后包含所有内容。|
|staticCodeValidation|Boolean|静态验证代码要求。 如果进程使动态代码签名失效，请使用此设置。|
|blockCamera|Boolean|阻止访问相机应用。|
|blockMicrophone|Boolean|阻止访问麦克风。|
|blockScreenCapture|Boolean|阻止应用捕获系统显示的内容。 需要 macOS 10.15 或更高版本。|
|blockListenEvent|Boolean|阻止应用或进程侦听来自输入设备（如鼠标、键盘和触控板）的事件。需要 macOS 10.15 或更高版本。|
|speechRecognition|[enablement](../resources/intune-shared-enablement.md)|允许或阻止访问系统语音识别设备。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|辅助功能|[enablement](../resources/intune-shared-enablement.md)|允许应用或进程通过辅助功能子系统控制 Mac。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|addressBook|[enablement](../resources/intune-shared-enablement.md)|允许或阻止访问由联系人管理的联系人信息。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|日历|[enablement](../resources/intune-shared-enablement.md)|允许或阻止访问日历管理的事件信息。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|reminders|[enablement](../resources/intune-shared-enablement.md)|允许或阻止对由提醒管理的信息的访问。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|photos|[enablement](../resources/intune-shared-enablement.md)|允许或阻止访问由照片管理的图像。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|mediaLibrary|[enablement](../resources/intune-shared-enablement.md)|允许或阻止访问音乐和媒体库。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|fileProviderPresence|[enablement](../resources/intune-shared-enablement.md)|允许应用或进程访问由另一个应用的文件提供程序扩展名管理的文件。 需要 macOS 10.15 或更高版本。 . 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicyAllFiles|[enablement](../resources/intune-shared-enablement.md)|控制对设备上所有受保护文件的访问。 文件可能位于电子邮件、邮件、应用和管理设置等位置。 请谨慎应用此设置。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicySystemAdminFiles|[enablement](../resources/intune-shared-enablement.md)|允许应用或进程访问系统管理中使用的文件。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicyDesktopFolder|[enablement](../resources/intune-shared-enablement.md)|允许或阻止访问桌面文件夹。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicyDocumentsFolder|[enablement](../resources/intune-shared-enablement.md)|允许或阻止对 Documents 文件夹的访问。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicyDownloadsFolder|[enablement](../resources/intune-shared-enablement.md)|允许或阻止访问"下载"文件夹。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicyNetworkVolumes|[enablement](../resources/intune-shared-enablement.md)|允许或阻止访问网络卷。 需要 macOS 10.15 或更高版本。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|systemPolicyRemovableVolumes|[enablement](../resources/intune-shared-enablement.md)|控制对设备上可移动卷（如外部硬盘驱动器）的访问。 需要 macOS 10.15 或更高版本。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|postEvent|[enablement](../resources/intune-shared-enablement.md)|控制对 CoreGraphics API 的访问，这些 API 用于将 CGEvents 发送到系统事件流。 可取值为：`notConfigured`、`enabled`、`disabled`。|
|appleEventsAllowedReceivers|[macOSAppleEventReceiver](../resources/intune-deviceconfig-macosappleeventreceiver.md) 集合|允许或拒绝应用或进程将受限制的 Apple 事件发送到其他应用或进程。 你需要知道接收应用或进程的标识符、标识符类型和代码要求。 该集合最多可包含 500 个元素。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSPrivacyAccessControlItem",
  "displayName": "String",
  "identifier": "String",
  "identifierType": "String",
  "codeRequirement": "String",
  "staticCodeValidation": true,
  "blockCamera": true,
  "blockMicrophone": true,
  "blockScreenCapture": true,
  "blockListenEvent": true,
  "speechRecognition": "String",
  "accessibility": "String",
  "addressBook": "String",
  "calendar": "String",
  "reminders": "String",
  "photos": "String",
  "mediaLibrary": "String",
  "fileProviderPresence": "String",
  "systemPolicyAllFiles": "String",
  "systemPolicySystemAdminFiles": "String",
  "systemPolicyDesktopFolder": "String",
  "systemPolicyDocumentsFolder": "String",
  "systemPolicyDownloadsFolder": "String",
  "systemPolicyNetworkVolumes": "String",
  "systemPolicyRemovableVolumes": "String",
  "postEvent": "String",
  "appleEventsAllowedReceivers": [
    {
      "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
      "codeRequirement": "String",
      "identifier": "String",
      "identifierType": "String",
      "allowed": true
    }
  ]
}
```



