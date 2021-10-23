---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 289ab81b4b7989d4d2326daa3808880aa19bd610
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60559312"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MeetingRegistration meetingRegistration = new MeetingRegistration();
meetingRegistration.subject = "Microsoft Ignite";
meetingRegistration.description = "Join us November 2–4, 2021 to explore the latest tools, training sessions, technical expertise, networking opportunities, and more.";
meetingRegistration.startDateTime = OffsetDateTimeSerializer.deserialize("2021-11-02T16:00:00+00:00");
meetingRegistration.endDateTime = OffsetDateTimeSerializer.deserialize("2021-11-04T12:00:00+00:00");
meetingRegistration.allowedRegistrant = MeetingAudience.EVERYONE;
LinkedList<MeetingSpeaker> speakersList = new LinkedList<MeetingSpeaker>();
MeetingSpeaker speakers = new MeetingSpeaker();
speakers.displayName = "Henry Ross";
speakers.bio = "Chairman and Chief Executive Officer";
speakersList.add(speakers);
MeetingSpeaker speakers1 = new MeetingSpeaker();
speakers1.displayName = "Hailey Clark";
speakers1.bio = "EVP";
speakersList.add(speakers1);
meetingRegistration.speakers = speakersList;
LinkedList<MeetingRegistrationQuestion> customQuestionsList = new LinkedList<MeetingRegistrationQuestion>();
MeetingRegistrationQuestion customQuestions = new MeetingRegistrationQuestion();
customQuestions.displayName = "Are you a developer?";
customQuestions.answerInputType = AnswerInputType.RADIO_BUTTON;
LinkedList<String> answerOptionsList = new LinkedList<String>();
answerOptionsList.add("Yes");
answerOptionsList.add("No");
customQuestions.answerOptions = answerOptionsList;
customQuestions.isRequired = true;
customQuestionsList.add(customQuestions);
MeetingRegistrationQuestion customQuestions1 = new MeetingRegistrationQuestion();
customQuestions1.displayName = "Where did you hear about us?";
customQuestions1.answerInputType = AnswerInputType.TEXT;
customQuestions1.isRequired = false;
customQuestionsList.add(customQuestions1);
MeetingRegistrationQuestionCollectionResponse meetingRegistrationQuestionCollectionResponse = new MeetingRegistrationQuestionCollectionResponse();
meetingRegistrationQuestionCollectionResponse.value = customQuestionsList;
MeetingRegistrationQuestionCollectionPage meetingRegistrationQuestionCollectionPage = new MeetingRegistrationQuestionCollectionPage(meetingRegistrationQuestionCollectionResponse, null);
meetingRegistration.customQuestions = meetingRegistrationQuestionCollectionPage;

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ").registration()
    .buildRequest()
    .post(meetingRegistration);

```